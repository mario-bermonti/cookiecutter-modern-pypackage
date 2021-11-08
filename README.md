# Cookiecutter Modern PyPackage

[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/mario-bermonti/cookiecutter-modern-pypackage?logo=github)](https://github.com/mario-bermonti/cookiecutter-modern-pypackage/releases)
[![Python Version](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue?logo=python)](https://www.python.org/)
[![License](https://img.shields.io/badge/license-MIT-brightgreen)](https://opensource.org/licenses/MIT)
[![Tests](https://github.com/mario-bermonti/cookiecutter-modern-pypackage/workflows/tests/badge.svg)](https://github.com/mario-bermonti/cookiecutter-modern-pypackage/actions?workflow=tests)
[![Read the Docs](https://readthedocs.org/projects/cookiecutter-modern-python-package/badge/?version=latest)](https://cookiecutter-modern-python-package.readthedocs.io)
[![Black](https://img.shields.io/badge/code%20style-black-000000)](https://github.com/psf/black)
[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)


[Cookiecutter][cookiecutter] template for a modern Python package.

* GitHub repo: <https://github.com/mario-bermonti/cookiecutter-modern-pypackage.git>
* Documentation: <https://cookiecutter-modern-python-package.readthedocs.io>
* Free software: MIT license

## Features

* Dependency tracking using [Poetry][poetry]
* Testing setup with [Pytest][pytest]
* [Github Actions][github actions] ready for Continuous Integration testing
* Linting provided by [Flake8][flake8] with [Flakehell][flakehell]
* Docstring linting provided by [Darglint][darglint] using the [Google Python Style Guide][google styleguide]
* Static type checking by [Mypy][mypy]
* Formatting provided by [Black][black] and [Isort][isort]
* Checks dependencies for known security vulnerabilities with [Safety][safety]
* Git hooks managed by [pre-commit][pre-commit].
* All development tasks (lint, format, test, etc) wrapped up in a python CLI by [invoke][invoke]
* Multiple Python environments testing provided by [Nox][nox]
* Documentation provided by [Sphinx][sphinx] ready for generation with, for example, [Read the Docs][rtd]
* Command line interface using [Click][click] (optional)
* Automated dependency updates with [Dependabot][dependabot]
* Coverage reports on [Codecov][codecov]
* Automated releases to [PyPI][pypi]  (optional)

## Quickstart

Install the latest Cookiecutter if you haven't installed it yet (this requires Cookiecutter 1.4.0 or higher):

```
pip install -U cookiecutter
```

Generate a Python package project:

```
cookiecutter gh:mario-bermonti/cookiecutter-modern-pypackage
```

Then:

* Create a repo and put it there.
* Install the dev requirements into a virtualenv. (`poetry install`)
* Install pre-commit hooks. (`poetry run inv install-hooks`)
* Configure [Codecov][codecov] repository settings. (Codecov App, `CODECOV_TOKEN`)
* Add the repo to your [Read the Docs][rtd] account + turn on the Read the Docs service hook.
* Configure [PyPI][pypi] token. (`PYPI_TOKEN`)
* Release your package by pushing a new tag.

For more details, see the [tutorial][tutorial].

## Contributing to this project
  All contributions are welcome!

  Will find a detailed description of all the ways you can contribute to cookiecutter-modern-pypackage in
  the [contributing guide][contributing_guide].

  This is a beginner-friendly project so don't hesitate to ask any questions or get in touch
  with the project's maintainers.

  Please review the [project's code of conduct][code_conduct] before making
  any contributions.

## Credits

This cookiecutter is a fork of [fedejaure's][original_cookie]
awesome python package template. It uses most of fedejaure's code and configuration,
but it has been adapted so it is easier to use by scientists who have limited
technical background in programming.

Please do checkout [fedejaure's][original_cookie] template as it is great and may even be better
suited for your needs.

This template is also influenced by these awesome projects:

* [audreyr/cookiecutter-pypackage][audreyr/cookiecutter-pypackage]: Cookiecutter template for a Python package.
* [briggySmalls/cookiecutter-pypackage][briggySmalls/cookiecutter-pypackage]: A fork from [audreyr/cookiecutter-pypackage][audreyr/cookiecutter-pypackage] using Poetry for package management, with linting, formatting and more.
* [hypermodern-python][hypermodern-python]: Hypermodern Python article series.
* [TezRomacH/python-package-template][tezromach]: Your next Python package needs a bleeding-edge project structure.

[cookiecutter]: https://github.com/cookiecutter/cookiecutter
[poetry]: https://python-poetry.org/
[pytest]: https://github.com/pytest-dev/pytest
[github actions]: https://github.com/features/actions
[flake8]: https://gitlab.com/pycqa/flake8
[flakehell]: https://github.com/life4/flakehell
[isort]: https://github.com/timothycrosley/isort
[black]: https://github.com/psf/black
[darglint]: https://github.com/terrencepreilly/darglint
[mypy]: https://github.com/python/mypy
[pre-commit]: https://pre-commit.com/
[safety]: https://github.com/pyupio/safety
[google styleguide]: https://google.github.io/styleguide/pyguide.html
[invoke]: https://www.pyinvoke.org/
[sphinx]: https://www.sphinx-doc.org/en/master/
[rtd]: https://readthedocs.org/
[nox]: https://nox.thea.codes/en/stable/
[tutorial]: https://cookiecutter-modern-pypackage.readthedocs.io/en/latest/tutorial.html
[click]: http://click.pocoo.org/
[dependabot]: https://dependabot.com/
[audreyr/cookiecutter-pypackage]: https://github.com/audreyr/cookiecutter-pypackage
[briggySmalls/cookiecutter-pypackage]: https://github.com/briggySmalls/cookiecutter-pypackage
[hypermodern-python]: https://cjolowicz.github.io/posts/hypermodern-python-01-setup/
[codecov]: https://codecov.io/
[pypi]: https://pypi.org/
[testpypi]: https://test.pypi.org/
[code_conduct]: ./CODE_OF_CONDUCT.md
[contributing_guide]: ./contributing.md
[original_cookie]: https://github.com/fedejaure/cookiecutter-modern-pypackage
[TezRomacH]: https://github.com/TezRomacH/python-package-template
