# django-tailwind-cli

![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/oliverandrich/django-tailwind-cli/test.yml?style=flat-square)
[![PyPI](https://img.shields.io/pypi/v/django-tailwind-cli.svg?style=flat-square)](https://pypi.org/project/django-tailwind-cli/)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
![GitHub](https://img.shields.io/github/license/oliverandrich/django-tailwind-cli?style=flat-square)
[![poetry-managed](https://img.shields.io/badge/poetry-managed-blue?style=flat-square)](https://python-poetry.org)

This project provides an integration of [Tailwind CSS](https://tailwindcss.com) for Django that is based on the precompiled versions of the [Tailwind CSS CLI](https://tailwindcss.com/blog/standalone-cli).

It is inspired by the implementation of the [Tailwind integration for Phoenix](https://github.com/phoenixframework/tailwind) which completely skips the neccesity of a node installation. So it is a perfect match, if you are a user of [htmx](https://htmx.org) or any other framework that tries to avoid JavaScript coding in your web app. My personal motivation was, that I discovered that I never needed any other plugin besides the official plugins, which are already included in the CLI.

> If you want to use node or you have to use it because of other dependencies, then the package [django-tailwind](https://github.com/timonweb/django-tailwind) by [Tim Kamamin](https://github.com/timonweb) might be a better solution for you.

## Features

- Management Commands...
  - ...to install the the CLI for your operating system and machine architecture.
  - ...to start the CLI in watch mode to incrementally compile your style sheet.
  - ...to create a theme app which includes a basic stylesheet and a tailwind configuration which you can extend.
  - ...to build the production ready CSS file.
- A template tag to include the CSS file in your base template.
- All the official plugins (typography, form, line-clamp, container queries, and aspect-ratio) integrated in the CLI are activated in the default configuration.

## Requirements

Python 3.8 or newer with Django >= 3.2.

## Installation

Follow the [installation instructions](/installation/) to set up the app in your project.

## License

This software is licensed under [MIT license](https://github.com/oliverandrich/django-tailwind-cli/blob/main/LICENSE). Copyright (c) 2022 [Oliver Andrich](https://andrich.me/).