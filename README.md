# ToDo List App

A Django learning project for creating, updating, and deleting tasks, with server-rendered templates and SQLite storage.

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?logo=django&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=white)
[![Stars](https://img.shields.io/github/stars/Aman6124/ToDo-list-App?style=flat)](https://github.com/Aman6124/ToDo-list-App/stargazers)
[![Forks](https://img.shields.io/github/forks/Aman6124/ToDo-list-App?style=flat)](https://github.com/Aman6124/ToDo-list-App/forks)

## Features

- View tasks in a single list.
- Add tasks using a Django form.
- Update existing task details.
- Confirm and delete tasks.
- Store records in SQLite.

## Attribution

This repository is a fork of [larymak/ToDo-list-App](https://github.com/larymak/ToDo-list-App). Credit for the original application belongs to its upstream contributors.

## Project structure

- `manage.py` — Django command entry point.
- `todo/` — application settings and root URL configuration.
- `tasks/models.py` — task data model.
- `tasks/forms.py` — task form.
- `tasks/views.py` — list, create, update, and delete handlers.
- `tasks/templates/tasks/` — HTML templates.
- `tasks/migrations/` — database migrations.

## Development status

The settings file identifies this as a Django 3.0.8-era project, and there is currently no dependency manifest. A supported Django/Python combination must be selected and tested before treating setup as reproducible.

The checked-in settings also have a placeholder secret key, `DEBUG = False`, and an empty `ALLOWED_HOSTS`. Configure a local development environment before starting the server.

## Getting started

Clone the default development branch:

```bash
git clone --branch v1.0 https://github.com/Aman6124/ToDo-list-App.git
cd ToDo-list-App
python -m venv .venv
```

Activate `.venv` for your shell and install a Django version compatible with the code. Configure a development secret key and allow `localhost` and `127.0.0.1` in your local settings.

Then run:

```bash
python manage.py check
python manage.py migrate
python manage.py runserver
```

Open [localhost:8000](http://localhost:8000).

## Contributing

Useful next steps include a tested dependency manifest, environment-based settings, and tests for task creation, updates, and deletion. Open an issue with reproduction steps or submit a focused pull request with the checks you ran.
