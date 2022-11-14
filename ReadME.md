docker and postgres

vesions in docker file
docker compose 3.9 
python 3.8
django 4.1.3

start project 
1. folder create
2. run this commands 
python -m venv venv
venv\scripts\activate
pip install -r requirements.txt
django-admin startproject config .
python manage.py runserver


set this code in settings  
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'postgres',
        'USER': 'postgres',
        'PASSWORD': 'postgres',
        'HOST': 'db',
        'PORT': 5432
    }
}