## Cheat Sheet

```
// Creating a new project
django-admin startproject projectname

//Add an app to a project
python3 manage.py startapp appname

//Starting the server
python3 manage.py runserver

//creating migrations 
python3 manage.py makemigrations

//migrate the database
python3 manage.py migrate

//creating a Super User for the admin panel
pyhton3 manage.py createsuperuser

//collecting static files into one folder
python3 manage.py collectstatic

//checking current version
python3
>>> import django
>>> django.VERSION
(2, 0, 0, 'final', 0)

```
## Downloading Django & Starting first project
```
pip3 install django //Newest verison
pip3 install django==2.0.2 //Specific verison

django-admin help
django-admin startproject firstProject // Create a new project

python3 manage.py runserver // Starts server 127.0.0.1:8000
```
## Python virtual environment
```
//Install pip3
sudo apt-get install -y python3-pip

//Install virtual env
sudo pip3 install virtualenv

//Create a new virtual environment
virtualenv venv

//Activate
source venv/bin/activate

//Deactivate
deactivate
```
## Setup and Existing Django Project
```
1. Grab a copy of the project
git clone new_project.git

2. Create a virtual environment and install dependencies
virtualenv venv
source venv/bin/activate
pip install -r requirements.txt

3. Duplicate
new_project/new_project/local_settings_example.py and save as local_settings.py.

4. Enter your database settings in local_settings.py.

5. Initialize your database.

python ./manage.py syncdb
python ./manage.py migrate
```