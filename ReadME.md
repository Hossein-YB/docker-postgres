#docker and postgres

<h6>vesions in docker file</h6>
docker compose 3.9 
python 3.8
django 4.1.3

#start project 
1. folder create<br>
2. run this commands</br> 
```python -m venv venv```
```venv\scripts\activate```
```pip install -r requirements.txt```
```django-admin startproject config .```
```python manage.py runserver```


#set this code in settings  
```
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
```
#<h4>app accounts for custome user model</h4>

set in settings file this varible
``` AUTH_USER_MODEL = 'accounts.CustomUser' ```
