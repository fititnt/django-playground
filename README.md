# django-playground


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
```