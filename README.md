# 🧪 Cookiecutter Python Project Template (test project)

A modern, minimal Cookiecutter template for Python projects using up-to-date tooling like `uv`, `ruff`, `mypy`, `pytest`, `pre-commit`, and `bandit`.

## 🚀 Quick Start

Install Cookiecutter (if not already installed):

Cookiecutter must be installed globally:

```bash
pip install pipx
pipx install cookiecutter
```

Generate a new project:

```bash
cookiecutter gh:tlamdchbh/cookiecutter-python-project
```
or 
```bash
cookiecutter gh:tlamdchbh/cookiecutter-python-project --output-dir [your folder]
```

Answer the prompts and a new project folder will be created.

## 🛠️ Template Features

- **uv** — fast dependency management
- **pyproject.toml** — unified configuration
- **pre-commit** — automated code quality checks
- **ruff** — linting and formatting
- **mypy** — static type checking
- **pytest** — unit testing
- **bandit** — security analysis

## ⚙️ Install Dependencies

```bash
uv pip install -e ".[dev]"
pre-commit install
```

## 🧪 Run Tests

```bash
pytest
```

## 🧹 Code Quality Checks

```bash
ruff .
mypy .
bandit -c pyproject.toml src/
```

## 🔐 GitHub Support (Optional)

During generation, you can choose whether the project will be hosted on GitHub. This affects:

- `README.md` content
- `pyproject.toml` links
- URLs to homepage and issue tracker

## 📝 License

Select during generation: MIT
