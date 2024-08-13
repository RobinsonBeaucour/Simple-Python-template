# {{ cookiecutter.project_name}}

{{ cookiecutter.package_description}}

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


## To install package

```shell
pip install {{ cookiecutter.project_slug }}
```

## To install dev set-up

```shell
pip install poetry
```

```shell
poetry install
```

### To run test with coverage report

```shell
poetry run pytest --cov {{ cookiecutter.project_slug }} --cov-report html
```

### To build documentation

```shell
cd docs
```

```shell
poetry run sphinx-build -M html . _build
```

### About notebooks

**Please number the notebooks.**

Please read [conversion guide](./notebooks/CONVERT.md) for html export.
