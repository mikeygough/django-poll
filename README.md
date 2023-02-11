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
