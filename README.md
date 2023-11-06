
# Tauth


### installation guide
 1. copy this tauth folder inside your root folder. 
 2. add this url in urls.py
 base code::
  ```
  path('auth/', include('tauth.urls')),
```
 

3. add this tauth in install app 

  ```
  INSTALLED_APPS = [
    .......
    'tauth',
]
```
add this DEFAULT_AUTHENTICATION_CLASSES 

```
REST_FRAMEWORK = {
    'DEFAULT_AUTHENTICATION_CLASSES': (
        'tauth.authentication.TAuthJWTAuthentication',
    ),
}
```
### migrate 

```
python manage.py makemigrations
python manage.py migrate

```

### Run 
```
python manage.py runserver
 ```









A brief description of what this project does and who it's for

