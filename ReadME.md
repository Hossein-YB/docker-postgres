#docker and postgres

<h6>vesions in docker file</h6>
docker compose 3.9 
python 3.8
django 4.1.3

#start project 
1. folder create<br>
2. run this commands</br> 
<code>python -m venv venv</code></br>
<code>venv\scripts\activate</code></br>
<code>pip install -r requirements.txt</code></br>
<code>django-admin startproject config .</code></br>
<code>python manage.py runserver</code></br>


#set this code in settings  
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