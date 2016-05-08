# Getting started

Ubuntu 16.04.

Create a new Django project:

    # TODO gives a use -H warning.
    sudo pip install --upgrade virtualenv
    virtualenv -p python3.5 .env
    # Check python version.
    #python --version
    . .env/bin/activate
    pip install -r requirements.txt

How to start a new Django project: first do the same as above, but instead of `pip install -r requirements.txt` do:

    pip install django
    # Check django version.
    # python -c "import django; print(django.get_version())"
    django-admin startproject NAME
    cd NAME
    pip freeze >requirements.txt
    python manage.py migrate
    python manage.py runserver
