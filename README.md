# Simple Python Template Cookiecutter

## Quickstart

Install the latest Cookiecutter if you haven't installed it yet (this requires
Cookiecutter 1.4.0 or higher):

    pip install -U cookiecutter

Generate a Python package project::

    cookiecutter https://github.com/RobinsonBeaucour/Simple-Python-template.git

The template follows the below structure :

------------

    ├── .gitignore                  <- Specifies files and directories that should be ignored by Git during version control.
    ├── AUTHORS.rst                 <- A file listing the authors of the project.
    ├── pyproject.toml              <- Configuration file used to specify project metadata, dependencies, build requirements, and other settings.
    ├── README.md                   <- The main documentation file providing an overview and usage instructions for the project.
    ├── {{ cookiecutter.project_slug }}                     <- Package directory for the main project code.
    ├── docs                        <- Directory containing documentation files.
    │   ├── authors.rst             <- Authors documentation.
    │   ├── conf.py                 <- Configuration file for Sphinx, a documentation generator.
    │   ├── index.rst               <- Main documentation index file.
    │   ├── installation.rst        <- Installation documentation.
    │   ├── make.bat                <- Batch file for building documentation on Windows.
    │   ├── Makefile                <- Makefile for building documentation.
    │   ├── readme.rst              <- Readme documentation.
    ├── docs                        <- Directory containing notebooks.    
    └── tests                       <- Directory containing test files.