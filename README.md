# Running Python Code

This repository contains the lesson materials and exercises for the "Running Python Code" lesson. It is a tiny starter project that demonstrates how to run Python programs, create a virtual environment, and run tests with pytest.

## Learning Goals

- Run Python code from a file
- Log output to the terminal
- Run Python code from the Python REPL (interactive shell)
- Create and use a `pipenv` virtual environment (or use `venv`/`virtualenv`)
- Run tests with `pytest`

## Prerequisites

- Python 3.8 or newer installed on your machine
- Git (to clone this repository)
- Optional: `pipenv` if you want to follow the pipenv workflow

## Quick start

Clone the repository and change into the project directory:

```bash
git clone git@github.com:Sam-Safari/python-p3-running-python-code.git
cd python-p3-running-python-code
```

Create and activate a `pipenv` environment (recommended for this lesson) and install dev dependencies:

```bash
pipenv install --dev
pipenv shell
```

If you prefer to use the standard library `venv`:

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt  # if a requirements file exists
```

## Run the example application

The repository includes a tiny example script at `lib/app.py`. Run it with:

```bash
python3 lib/app.py
# or, inside pipenv:
pipenv run python lib/app.py
```

You should see:

```text
Hello World! Pass this test, please.
```

## Run the tests

If you used `pipenv install --dev` (or installed pytest in your environment) run:

```bash
pytest
# or inside pipenv
pipenv run pytest
```

## Project structure

- `lib/` - example application code
  - `app.py` - tiny script used by the lesson/tests
- `testing/` - test files and pytest fixtures used by the course
- `README.md` - this file

## Contributing

If you'd like to contribute, fork the repository, make your changes on a branch, and open a pull request. Keep changes small and focused.

## License

This repository is provided under the terms of the repository license (see `LICENSE.md`).

