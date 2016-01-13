# Getting started

Install Python 3, preferably with `virtualenv`, then:

    sudo pip install --upgrade virtualenv
    virtualenv -p python3.4 .env
    . .env/bin/activate
    django-admin startproject NAME
    cd NAME
    python manage.py migrate
    python manage.py runserver
