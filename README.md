# AWS Deployment - Django App

  
  * Django Authentication - with Mysql
## Django Polls App - with Mysql

1. Ensure that mysql is installed, python3 and django for polls app - mysite folder.

  * [Python3](https://www.python.org/downloads/)

  * [Django](https://docs.djangoproject.com/en/2.0/topics/install/#installing-official-release)

  * [Mysql](https://dev.mysql.com/downloads/mysql/)
  
  * [Heroku](https://devcenter.heroku.com/articles/getting-started-with-python#introduction)

2.git clone this repository
```
git clone https://github.com/heroku/python-getting-started.git

```

3.create account on heroku
```
heroku login 

heroku create

git push heroku master

heroku open
```

## Django Authentication - with Mysql

1.Create user from the command line
```
heroku run python manage.py createsuperuser
```

3.run migrations
```
heroku run python manage.py migrate

```
4.run the server
```
heroku run python manage.py runserver
```
5. check the logs on heroku
```
heroku logs --tail
```
