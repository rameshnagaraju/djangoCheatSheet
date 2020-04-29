# setting up:

## Create virtual environment

- pipenv install --python python3

### To activate

- pipenv shell.

### To deactivate

- exit

# commands to verify django version

1. python -m django --version

# Create a new project:

- django-admin startproject myblog

# To run the project:

- pyhton manage.py runserver

# To create an app

- python manage.py startapp blog

# Migration commands

- python manage.py makemigrations
- python manage.py migrate
- python manage.py createsuoeruser
