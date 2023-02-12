# django-poll
learning a bit of django. following along with the getting started demo...

### create a project
_$_ django-admin startproject mysite

_$_ cd mysite

#### start the development server
_$_ python3 manage.py runserver

#### create the polls _app_ inside the mysite _project_
_$_ python3 manage.py startapp polls

#### add a view
#### create a urls.py file inside /polls
#### point the root URLconf at the polls.urls module

### database setup
#### create tables in the database 
_$_ python3 manage.py migrate

#### create models
#### run migration
_$_ python3 manage.py makemigrations polls

#### check out what SQL the migration would run
_$_ python3 manage.py sqlmigrate polls 0001

#### run migrate to create model tables in the database
_$_ python3 manage.py migrate

remember the three-step guide to making model changes:
1. change your models (in models.py)
2. run 'python3 manage.py makemigrations' to create migrations for those changes
3. run 'python3 manage.py migrate' to apply those changes to the database

### create an admin user
_$_ python3 manage.py createsuperuser
admin, admin@example.com, admin

### views
each view is responsible for doing one of two things: returning an HttpResponse object containing
the content for the requested page, or raising an exception such as Http404.

### reference:

#### virtual environments
Create a Python3 Virtual Environment: 
```python3 -m venv env```

Activate the Virtual Environment:
```source env/bin/activate```

Deactivate the Virtual Environment:
```deactivate```

To Remove a Virtual Environment:
```sudo em -rf venv```

#### requirements.txt
Automagically create a requirements.txt file:
```pip3 freeze > requirements.txt```
