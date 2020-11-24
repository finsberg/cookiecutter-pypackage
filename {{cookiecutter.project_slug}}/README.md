{% set is_open_source = cookiecutter.open_source_license != 'Not open source' -%} 

# {{ cookiecutter.project_name }}

{% if is_open_source %} 

[![image](https://img.shields.io/pypi/v/{{ cookiecutter.project_slug }}.svg)](https://pypi.python.org/pypi/{{ cookiecutter.project_slug }})

[![Documentation Status](https://readthedocs.org/projects/{{ cookiecutter.project_slug }}/badge/?version=latest)](https://ldrb.readthedocs.io/en/latest/?badge=latest)

{%- endif %}

![CI](https://github.com/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}/workflows/CI/badge.svg)



{{ cookiecutter.project_short_description }}

{% if is_open_source %} 
* Free software: {{ cookiecutter.open_source_license }} 
* Documentation: https://{{ cookiecutter.project_slug | replace("_", "-") }}.readthedocs.io.
{% endif %}

# Features

-   TODO

# Credits

This package was created with
[Cookiecutter](https://github.com/audreyr/cookiecutter) and the
[finsberg/cookiecutter-pypackage](https://github.com/finsberg/cookiecutter-pypackage)
project template.
