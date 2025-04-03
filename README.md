# 🧪 Cookiecutter Python Project Template (test project)

A modern, minimal Cookiecutter template for Python projects using up-to-date tooling like `uv`, `ruff`, `mypy`,
`pytest`, `pre-commit`, and `bandit`.

---

## 🚀 Quick Start: Cookiecutter Project Setup with `uv`

### 1. 🛠 Install Prerequisites

Install `pipx` (if not installed, globally!):

```bash
pip install pipx
```

Install `uv` (recommended method):

```powershell
powershell -ExecutionPolicy Bypass -Command "irm https://astral.sh/uv/install.ps1 | iex"
```

Install `cookiecutter` globally via `uv`:

```bash
pipx install -g cookiecutter
```

---

### 2. 📦 Generate a Project

Use your preferred template:

```bash
cookiecutter gh:tlamdchbh/cookiecutter-python-project.git
```

Follow the prompts to customize your project.

---

### 3. 🧱 Set Up Virtual Environment

Navigate to your new project folder:

```bash
cd your_project_folder
```

Create a virtual environment with a specific Python version (e.g., 3.8):

```bash
uv venv --python 3.8 .venv
```

Activate the environment:

```bash
.venv\Scripts\activate  # Windows
```

---

### 4. 📥 Install Dependencies

Install all project and development dependencies:

```bash
uv pip install -e ".[dev]"
```

---

### 5. 🧠 Configure PyCharm (Optional but Recommended)

- Open the project in PyCharm
- Go to `File > Settings > Python Interpreter`
- Click ⚙ → `Add...` → `Existing environment`
- Select:  
  ```
  <project-root>\.venv\Scripts\python.exe
  ```

---

### 6. ✅ Run Checks and Tests

Make sure everything is set up correctly:

```bash
python --version
ruff check .
mypy .
pytest
```

---

## ✅ Summary

---

| Action                             | Where to Perform | Instruction                                                                                          |
|------------------------------------|------------------|------------------------------------------------------------------------------------------------------|
| Install `pipx`                     | CMD              | `pip install pipx`                                                                                   |
| Install `uv`        | CMD              | `powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1                         | iex"` (once globally)                                                    |
| Install `cookiecutter`       | CMD              | `pipx pip install -g cookiecutter` (once globally)                                                   |
| Generate project                   | CMD              | `cookiecutter gh:tlamdchbh/cookiecutter-python-project.git` and follow prompts                       |
| Create/activate `.venv`            | CMD              | `uv venv --python [version] .venv` → then `.venv\Scripts\activate`                                 |
| Install dependencies               | CMD              | `uv pip install -e ".[dev]"`                                                                         |
| Connect interpreter to project     | PyCharm          | `Settings > Python Interpreter > Add... > Existing environment` → point to `.venv\Scripts\python.exe` |
| Development, execution, and testing | PyCharm          | Use built-in editor, terminal, run/debug, `pytest`, etc.                                             |

---

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
