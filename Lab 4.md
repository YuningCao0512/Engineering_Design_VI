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

The next step is to edit settings.py in ~/stevens/stevens. I add an asterisk to ALLOWED_HOSTS and 'myapp' to INSTALLED_APPS. I used command `nano ~/stevens/stevens/settings.py`.

![modified settings](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab4_pictures/nano_settings.png)

The next step is to copy `urls.py` to ~/stevens/stevens.
- `cp ~/iot/lesson4/stevens/urls.py .`

Then, copy admin.py, models.py, and views.py to ~/stevens/myapp.
- `cd myapp`
- `ls`
- `cp ~/iot/lesson4/stevens/admin.py .`
- `cp ~/iot/lesson4/stevens/models.py .`
- `cp ~/iot/lesson4/stevens/views.py .`

Then, copy index.html. 
- `mkdir static templates`
- `cd templates`
- `mkdir myapp`
- `cd myapp`
- `cp ~/iot/lesson4/stevens/index.html .`

![copy](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab4_pictures/stevens%20copying.png)

The next step is to enable Google Maps API. This is completed from Google Cloud Console and I got an API key. The next step is substitute YOUR_API_KEY in index.html with the API key (AIzaSyCceqju5x3Ay1sAs8wwVX7uKQQbAmcDczQ)
- `nano index.html`

![change API key](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab4_pictures/change%20API%20key.png)

Then, copy static files. 
- `cd ~/stevens/myapp/static`
- `cp ~/iot/lesson4/static/favicon.ico .`
- `mkdir myapp`
- `cd myapp`
- `cp ~/iot/lesson4/static/*css .`
- `cp ~/iot/lesson4/static/*js .`

![change files](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab4_pictures/stevens%20copy%20static%20files.png)

Updating database:
- `python3 manage.py makemigrations myapp`
- `python3 manage.py migrate`
- `python3 manage.py createsuperuser`

![data update](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab4_pictures/stevens%20data%20update.png)

I will use `python3 manage.py runserver` to run Django server.

![running](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab4_pictures/stevens%20running.png)
![admin](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab4_pictures/stevens%20Ajango.png)




















