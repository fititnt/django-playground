# django-playground
**Rocha's playground for Django (https://www.djangoproject.com/). Not really
useful for other, it's just me playing around a new framework/language for me**.

## Step by step (Django part)

```bash
### Tutorial Writing your first Django app, START ______________________________
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

# @see https://docs.djangoproject.com/en/3.0/intro/tutorial05/ (automated testing)
# (...)

# Command to test polls
python manage.py test polls

# @see https://docs.djangoproject.com/en/3.0/intro/tutorial06/ (static files)
# (...)

# @see https://docs.djangoproject.com/en/3.0/intro/tutorial07/
# (...)

# to see where base django templates where stored
python -c "import django; print(django.__path__)"

### Tutorial Writing your first Django app, ended! _____________________________

### Advanced tutorial: How to write reusable apps, start _______________________
# @see https://docs.djangoproject.com/en/3.0/intro/reusable-apps/
cd django-polls
python setup.py sdist

cd ..

# Install
python -m pip install --user django-polls/dist/django-polls-0.1.tar.gz

# Remove
python -m pip uninstall django-polls

### Advanced tutorial: How to write reusable apps, ended! ______________________
```

- **URLs**
  - <http://127.0.0.1:8000/polls/>
  - <http://127.0.0.1:8000/admin/>

## Step by step (Docker part)

```bash
# @see https://docs.docker.com/compose/django/
# (...)
docker-compose up
```

- **URLs** (via docker)
  - <http://127.0.0.1:8000/polls/>
  - <http://127.0.0.1:8000/admin/>
