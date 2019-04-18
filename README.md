## Django project layout example

# Steps to reproduce

This is a minimal Django 1.11 project. It was created with these steps:

1. Create a virtualenv
2. Manually install Django and other dependencies
3. `pip freeze > requirements.txt`
4. `django-admin startproject project .`
5. Update `project/settings.py` to configure `SECRET_KEY`, `DATABASE` and `STATIC_ROOT` entries
6. `./manage.py startapp welcome`, to create the welcome page's app

From this initial state you can:

- create new Django apps
- update settings to suit your needs
- install more Python libraries and add them to the `requirements.txt` file

### Database configuration

The sample application code and templates in this repository contain database connection settings and credentials that rely on being able to use **sqlite**.

## Local development

To run this project in your development machine, follow these steps:

1. (optional) Create and activate a [virtualenv](https://virtualenv.pypa.io/) (you may want to use [virtualenvwrapper](http://virtualenvwrapper.readthedocs.org/)).

2. Install dependencies:

   `pip install -r requirements.txt`

3. Create a development database:

   `./manage.py migrate`

4. If everything is alright, you should be able to start the Django development server:

   `./manage.py runserver`

5. Open your browser and go to http://127.0.0.1:8000, you will be greeted with a welcome page.
