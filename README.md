# Tweeter (Django)

A minimal Twitter-style microblog built with Django — users register, log in, and post short tweets with optional photos.

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?logo=django&logoColor=white)

## Overview

Tweeter was originally developed inside a Django projects collection and now lives in its own repository. It covers the core of a social posting app: authentication, a Tweet model with image uploads, and template-based feeds.

## Key Features

- **Tweet model** — user, text (max 255 chars), optional photo, created/updated timestamps
- Built-in Django authentication (register / login / logout)
- Photo uploads with Django media handling
- Template-based UI for posting and viewing tweets

## Tech Stack

Python · Django · SQLite · HTML templates · Pillow

## Project Structure

```
├── tweeter/    # Project settings, URLs, WSGI/ASGI
├── tweet/      # App: Tweet model, views, forms, URLs
├── templates/  # Feed, login, register and form templates
└── manage.py
```

## Getting Started

```bash
git clone https://github.com/datascientist970/tweeter-django.git
cd tweeter-django
python -m venv venv && source venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

## Notes

- The development database (`db.sqlite3`) and uploaded media are intentionally not tracked — run `migrate` to create a fresh database.
- This project was split out of the `Web-Development-Django-` collection into its own repository.

## Author

**Muhammad Dawood** — AI & Data Science Engineer | Full-Stack Developer
GitHub: https://github.com/datascientist970 · LinkedIn: https://www.linkedin.com/in/dawood406/
Mardan, Khyber Pakhtunkhwa, Pakistan
