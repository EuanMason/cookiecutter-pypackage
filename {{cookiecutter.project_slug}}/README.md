{% set is_open_source = cookiecutter.open_source_license != 'Not open source' -%}

# {{ cookiecutter.project_name }}

{% if is_open_source %}
[![pypi](https://img.shields.io/pypi/v/{{ cookiecutter.project_slug }}.svg)](https://pypi.org/project/{{ cookiecutter.project_slug }}/) {{ mdl-disable "<!-- markdownlint-disable MD034 -->" }}
[![python](https://img.shields.io/pypi/pyversions/{{ cookiecutter.project_slug }}.svg)](https://pypi.org/project/{{ cookiecutter.project_slug }}/) {{ mdl-disable "<!-- markdownlint-disable MD034 -->" }}
[![Build Status](https://github.com/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}/actions/workflows/dev.yml/badge.svg)](https://github.com/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}/actions/workflows/dev.yml) {{ mdl-disable "<!-- markdownlint-disable MD034 -->" }}
[![codecov](https://codecov.io/gh/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}/branch/main/graphs/badge.svg)](https://codecov.io/github/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}) {{ mdl-disable "<!-- markdownlint-disable MD034 -->" }}

{% else %}
{% endif %}

{{ cookiecutter.project_short_description }}

{% if is_open_source %}

* Documentation: <https://{{ cookiecutter.github_username }}.github.io/{{ cookiecutter.project_slug }}>
* GitHub: <https://github.com/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}> {{ mdl-disable "<!-- markdownlint-disable MD034 -->" }}
* PyPI: <https://pypi.org/project/{{ cookiecutter.project_slug }}/> {{ mdl-disable "<!-- markdownlint-disable MD034 -->" }}
* Free software: {{ cookiecutter.open_source_license }}
{% endif %}

## Features

* TODO

## Credits

This package was created with [CookieCutter](https://github.com/euanmason/cookiecutter-pypackage) which is based on [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter) and the [waynerv/cookiecutter-pypackage](https://github.com/waynerv/cookiecutter-pypackage) project template.
