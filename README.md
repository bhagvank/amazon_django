# AWS Deployment - Django App

  
  * Django Authentication - with Mysql
## Prerequisites

  * [Python](https://www.python.org/downloads/)

  * [Django](https://docs.djangoproject.com/en/2.0/topics/install/#installing-official-release)

  * [Mysql](https://dev.mysql.com/downloads/mysql/)
  
  * [AWS](https://aws.amazon.com)
1.create account on aws, ec2 node, security groups (http & ssh rules) and get the key -pair

2.Python and Django Setup
```
sudo yum install python-pip python-dev python-django
```

3.git clone this repository
```
git clone https://github.com/bhagvank/amazon_django.git

```

4. ssh to ec2 node..
```

ssh -i secret/key-pair_name.pem ec2user@IP-ADDRESS
```

5. Install Maria DB or Mysql 
```
sudo yum install mysql-server libmysqlclient-dev
```
6.login to mysql by:
```
      mysql -uroot

      mysql> CREATE DATABASE registration CHARACTER SET UTF8;
      
      mysql> create user 'newuser' identified by 'newuser';

      mysql> grant all privileges on registration.* to 'newuser';
      
```  
7. Run migrations
```
python manage.py migrate
```
## Django Authentication - with Mysql

1.Create user from the command line
```
python manage.py createsuperuser

```

3.run migrations
```
python manage.py migrate

```
4.run the server
```
python manage.py runserver
```

