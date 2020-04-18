# django-playground

> TODO: Feito até 4. Ir até parte 5 e depois https://docs.djangoproject.com/en/3.0/intro/tutorial05/

## Step by step

```bash
# @see https://docs.djangoproject.com/en/3.0/intro/tutorial01/

# Install
python -m pip install Django

# Start project
django-admin startproject playground

# Run migrations
python manage.py migrate

# Start server
python manage.py runserver

# Create polls app (dir pools/)

python manage.py createsuperuser
##  Username (leave blank to use 'fititnt'): admin
## Email address: demo@example.com
##  Password: pass
##  Password (again): pass
##  This password is too short. It must contain at least 8 characters.
##  This password is too common.
##  Bypass password validation and create user anyway? [y/N]: y   
##  Superuser created successfully.

python manage.py makemigrations polls
python manage.py migrate

# @see https://docs.djangoproject.com/en/3.0/intro/tutorial02/
# (...)

# @see https://docs.djangoproject.com/en/3.0/intro/tutorial03/
# (...)

# @see https://docs.djangoproject.com/en/3.0/intro/tutorial04/
# (...)

# Code to test polls
python manage.py test polls
```