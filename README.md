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

# Adding Static content
- create "static" folder in root directory
    - create css folder
        - create base.css file
        - create about.css file etc ....
    - create js folder
    - create images folder
- configure django 
    - Goto projrct settings.py, 
    -  Add STATICFILES_DIRS = [ OS.path.join (BASE_DIR, 'static')]
    -  In the HTML files , add a tag at the top of file ** {% load static %} **
    -  from here on any reference to static files shall be prefixed with ** href = "{% static '/cass/base.css '%}" **