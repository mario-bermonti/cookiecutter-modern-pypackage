{% set is_open_source = cookiecutter.open_source_license != 'Not open source' %}
# {{ cookiecutter.project_title }}

{% if is_open_source %}
[![PyPI - Version](https://img.shields.io/pypi/v/{{ cookiecutter.project_name }}.svg)](https://pypi.python.org/pypi/{{ cookiecutter.project_name }})
[![PyPI - License](https://img.shields.io/pypi/l/{{ cookiecutter.project_name }}.svg)](https://pypi.python.org/pypi/{{ cookiecutter.project_name }})
[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/{{ cookiecutter.project_name }}.svg)](https://pypi.python.org/pypi/{{ cookiecutter.project_name }})
[![Tests](https://github.com/{{ cookiecutter.github_username }}/{{ cookiecutter.project_name }}/workflows/tests/badge.svg)](https://github.com/{{ cookiecutter.github_username }}/{{ cookiecutter.project_name }}/actions?workflow=tests)
[![Codecov](https://codecov.io/gh/{{ cookiecutter.github_username }}/{{ cookiecutter.project_name }}/branch/master/graph/badge.svg?token=YOURTOKEN)](https://codecov.io/gh/{{ cookiecutter.github_username }}/{{ cookiecutter.project_name }})
[![Read the Docs](https://readthedocs.org/projects/{{ cookiecutter.project_name }}/badge/?version=latest)](https://{{ cookiecutter.project_name }}.readthedocs.io/en/latest/)
[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
{% endif %}

{{ cookiecutter.project_short_description }}

{% if is_open_source %}
* GitHub repo: <https://github.com/{{ cookiecutter.github_username }}/{{ cookiecutter.project_name }}.git>
* Documentation: <https://{{ cookiecutter.project_name }}.readthedocs.io/en/latest/>
* Free software: {{ cookiecutter.open_source_license }}
{% endif %}

## Features

* TODO

## Quickstart

TODO

## Contributing to this project
  All contributions are welcome!

  Will find a detailed description of all the ways you can contribute to {{ cookiecutter.project_name }} in
  [the contributing guide][contributing_guide].

  This is a beginner-friendly project so don't hesitate to ask any questions or get in touch
  with the project's maintainers.

  Please review the [project's code of conduct][code_conduct] before making
  any contributions.


## Credits

This package was created with [Cookiecutter][cookiecutter] and the [mario-bermonti/cookiecutter-modern-pypackage][cookiecutter-modern-pypackage] project template.

[cookiecutter]: https://github.com/cookiecutter/cookiecutter
[cookiecutter-modern-pypackage]: https://github.com/mario-bermonti/cookiecutter-modern-pypackage

[contributing_guide]: ./contributing.md
