# {{ cookiecutter.project_name }}

{{ cookiecutter.description }}

## Installation

```bash
# Install using pip
pip install {{ cookiecutter.package_name }}

# Install using uv
uv pip install {{ cookiecutter.package_name }}
```

## Development

This project uses modern Python tooling:
- uv for dependency management
- ruff for linting and formatting
- mypy for static type checking
- pytest for testing
- pre-commit hooks for quality assurance
- bandit and safety for security

### Setup development environment

```bash
# Clone the repository
git clone https://github.com/username/{{ cookiecutter.project_name }}.git
cd {{ cookiecutter.project_name }}

# Install dependencies with uv
uv pip install -e ".[dev]"

# Setup pre-commit hooks
pre-commit install
```

## License

MIT
