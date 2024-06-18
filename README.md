# Getting Started with Poetry
## A Python Dependency Management and Packaging Tool

Poetry is a tool for dependency management and packaging in Python. It allows you to declare the libraries your project depends on and it will manage (install/update) them for you.

Poetry also allows you to package your project into a distributable format (e.g. wheel, sdist, etc.) and publish it to PyPI.

In this tutorial, we will learn how to install Poetry, create a new Python project, add dependencies, and package and publish the project to PyPI.

## Set Up Poetry
To install Poetry, run the following command:

```bash
curl -sSL https://install.python-poetry.org | python3 -
```

This command will download and install Poetry on your system.

To verify that Poetry has been installed successfully, run the following command:

```bash
poetry --version
```

To create a new Python project using Poetry, run the following command:

```bash
poetry new my_project
```

This command will create a new directory called `my_project` with the following structure:

```plaintext
my_project
├── my_project
│   └── __init__.py
├── pyproject.toml
└── tests
	├── __init__.py
	└── test_my_project.py
```

The `pyproject.toml` file is the configuration file for the project. It contains the project's metadata and dependencies.

To add a dependency to the project, run the following command:

```bash
poetry add requests
```

This command will add the `requests` library as a dependency to the project.

To package the project, run the following command:

```bash
poetry build
```

This command will create a distributable package (e.g. wheel, sdist) for the project.

To publish the project to PyPI, run the following command:

```bash
poetry publish
```

This command will publish the project to PyPI.


