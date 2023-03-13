# Python Repository Template

[![Python 3.10][python_badge]](https://www.python.org/downloads/release/python-3106/)
[![License: AGPL v3][agpl3_badge]](https://www.gnu.org/licenses/agpl-3.0)
[![Code Style: Black][black_badge]](https://github.com/ambv/black)

Example Python repository to quickly fork into new clean environment.

- typechecking
- pre-commit

## Usage

First install this pip package with:

```bash
pip install pythontemplate
```

Then run:

```py
python -m src.pythontemplate
```

## Developer

```bash
pre-commit install
pre-commit autoupdate
pre-commit run --all
```

## Publish pip package

Build the pip package with:

```bash
pip install --upgrade pip setuptools wheel
pip install twine
```

Install the pip package locally with:

```bash
pip install -e .
```

Upload the pip package to the world with:

```bash
rm -r dist
rm -r build
python3 setup.py sdist bdist_wheel
python3 -m twine upload dist/\*
```

<!-- Un-wrapped URL's below (Mostly for Badges) -->

[agpl3_badge]: https://img.shields.io/badge/License-AGPL_v3-blue.svg
[black_badge]: https://img.shields.io/badge/code%20style-black-000000.svg
[python_badge]: https://img.shields.io/badge/python-3.6-blue.svg
