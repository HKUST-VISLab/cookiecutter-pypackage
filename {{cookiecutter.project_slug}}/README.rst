<p align="left">
<img width=15% src="http://vis.cse.ust.hk/vislab_homepage/img/logo_tmp01.png" alt=“VisLab” />
<i>An open source project from VisLab at HKUST.</i>
</p>

<!-- Uncomment these lines after releasing the package to PyPI for version and downloads badges -->
[![PyPI Shield](https://img.shields.io/pypi/v/{{ cookiecutter.package_name }}.svg)](https://pypi.python.org/pypi/{{ cookiecutter.package_name }})
[![Downloads](https://pepy.tech/badge/{{ cookiecutter.package_name }})](https://pepy.tech/project/{{ cookiecutter.package_name }})


# {{ cookiecutter.project_name }}

{{ cookiecutter.project_short_description }}

{% if cookiecutter.open_source_license == 'Not open source' -%}
- Free software: {{ cookiecutter.open_source_license }}
{% endif -%}
- Documentation: https://{{ cookiecutter.github_owner }}.github.io/{{ cookiecutter.repository_name }}
- Homepage: https://github.com/{{ cookiecutter.github_owner }}/{{ cookiecutter.repository_name }}

# Overview

TODO: Provide a short overview of the project here.

## Online Demos

TODO: (optional) Create online system demos to enable users to try the system themselves.



# Install

## Requirements

**{{ cookiecutter.project_name }}** has been developed and tested on [Python {% if cookiecutter.support_py2 == 'y' %}2.7, {% endif %}3.7 and 3.8](https://www.python.org/downloads/)

Also, although it is not strictly required, the usage of a [virtualenv](https://virtualenv.pypa.io/en/latest/)
is highly recommended in order to avoid interfering with other software installed in the system
in which **{{ cookiecutter.project_name }}** is run.

These are the minimum commands needed to create a virtualenv using python3.7 for **{{ cookiecutter.project_name }}**:

```bash
pip install virtualenv
virtualenv -p $(which python3.7) {{ cookiecutter.repository_name }}-venv
```

Afterwards, you have to execute this command to activate the virtualenv:

```bash
source {{ cookiecutter.repository_name }}-venv/bin/activate
```

Remember to execute it every time you start a new console to work on **{{ cookiecutter.project_name }}**!

<!-- Uncomment this section after releasing the package to PyPI for installation instructions
## Install from PyPI

After creating the virtualenv and activating it, we recommend using
[pip](https://pip.pypa.io/en/stable/) in order to install **{{ cookiecutter.project_name }}**:

```bash
pip install {{ cookiecutter.package_name }}
```

This will pull and install the latest stable release from [PyPI](https://pypi.org/).
-->

## Install from source

With your virtualenv activated, you can clone the repository and install it from
source by running `make install`:

```bash
git clone git@github.com:{{ cookiecutter.github_owner }}/{{ cookiecutter.repository_name }}.git
cd {{ cookiecutter.repository_name }}
make install
```

# Getting Started

In this short tutorial we will use some examples to help you
getting started with **{{ cookiecutter.project_name }}**.

TODO: Create a step by step guide here

# Learn More

For more details about **{{ cookiecutter.project_name }}**, please check the [documentation site](
https://{{ cookiecutter.github_owner }}.github.io/{{ cookiecutter.repository_name }}/).

# Citation

If you find this repository helpful, please do consider citing our publication [{{ cookiecutter.pub_name }}]({{ cookiecutter.pub_link }})

```
TODO: add BibTeX
```

# Contributing

Please read [Contributing Guide](https://{{ cookiecutter.github_owner }}.github.io/{{ cookiecutter.project_slug }}/CONTRIBUTING.rst)
for more details about this process.

# Licence

This project is licensed under the {{ cookiecutter.open_source_license }} - see the [LICENSE](https://{{ cookiecutter.github_owner }}.github.io/{{ cookiecutter.project_slug }}/LICENSE) file for details.