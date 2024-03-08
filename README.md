## Configurações inicias de um projeto Python

## Instalação do Poetry

``pip install poetry``

# Iniciar um novo projeto

``poetry new nome_do_projeto``
``cd new nome_do_projeto``

## Instalação do virtualenv

``pip install virtualenv``

``python -m virtualenv .venv``

``.venv\Scripts\activate``

# Instalação das dependencias pelo Poetry

- Lint com black

``poetry add black``

- Lint com flake8

`` poetry add flake8``

- Tasks

`` poetry add taskipy``

## Configuração do taskipy

``
[tool.taskipy.tasks]
test = "python -m unittest tests/test_*.py"
lint_flake = "flake8 init_python_configuration"
lint_black = "black --check init_python_configuration"``

## Comandos de utilização do taskipy

``task test``

``task lint_flake``

``task lint_black``

## Instalação do mkdocs
poetry add mkdocs
poetry add "mkdocstrings[python]"
poetry add mkdocs-material 

mkdocs new [dir-name] - Create a new project.
mkdocs serve - Start the live-reloading docs server.
mkdocs build - Build the documentation site.
mkdocs -h - Print help message and exit
