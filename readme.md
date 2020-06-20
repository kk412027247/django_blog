
```shell script
          
python3 manage.py makemigrations blog

python3 manage.py migrate
                       
python3 manage.py runserver

python3 manage.py shell

```

#### create a user for your PostgreSQL database

```shell script  
sudo bash
su postgres 
createdb -E utf8 -U blog -h 127.0.0.1 blog   
```

```python 
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'blog',
        'USER':'blog',
        'PASSWORD':'123456',
        'HOST':'127.0.0.1'
    }
}

```


# create a superuser

```shell script 
python3 manage.py createsuperuser
  
```
