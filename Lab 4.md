# Lab 4: Django and Flask
The main purposes of this lab will be:
- Install Django and Django REST framework
- Use the default database, i.e., SQLite
- Start Django project "stevens," run server, and view app
- Start Django REST project "mycpu," run server, and view app
- Install Flask if no module named 'flask'
- Run Flask server via hello_world.py and view app

[Reference recourses](https://github.com/kevinwlu/iot/tree/master/lesson4)

---
## 1. Django and Django REST framework
I will install Django and Django REST framework at this session. 
- `pip3 -V`
- `pip3 list`
- `pip3 install -U setuptools`
- `pip3 install -U django`
- `pip3 install -U djangorestframework`
- `pip3 install -U django-filter`
- `pip3 install -U markdown`
- `pip3 install -U requests`

All libraries are downloaded with the commands above.

---
## 2. Start Django and running servers 
At this session, I will use the default database (i.e., SQLite); start Django project "stevens," run server, and view app; start Django REST project "mycpu," run server, and view app. 
By default, Django uses SQLite. 

### stevens 
To start the project "stevens", I used to the following commands:

- `django-admin startproject stevens`
- `cd stevens`
- `ls`

![starting stevens](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab4_pictures/starting%20stevens%20.png)

The following commands give instructions on how to start a Django app:
- `python3 manage.py startapp myapp`
- `ls`

The output can be displayed:

![app stevens](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab4_pictures/stevens%20app%20.png)

The next step is to edit settings.py in ~/stevens/stevens. I add an asterisk to ALLOWED_HOSTS and 'myapp' to INSTALLED_APPS. I used command `nano settings.py`.










