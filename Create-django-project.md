# Create a Django project

You need a couple of things before you can create a django project directly.
First you need to set up a Virtual Enviroment to setup django and it's components inside of it,
And for that we are going to install Homebrew (The Missing Package Manager for macOS).
Why do we need Homebrew?
It's simple, to install python 3 and it's packages to make our life easer,
Do to mac os still uses python 2.

After installing Homebrew and Python3 we are going to set up our folder and setup the Virtual Enviroment.

**So LET'S GO!**

## The things we need to work with DJANGO

1. xcode command line tools
2. Homebrew
3. python3
4. postgresql(or any database)

## Xcode command line tools

- Install tools

```bash
 xcode-select --install 
```

## Homebrew

1. Install Homebrew in your Terminal

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

2. Check Homebrew version

```bash
 brew --version
```

## Python3

1. Install Python3 in your Terminal

```bash
brew install python
```

2. Check python version

```bash
 python3 --version
```

## Postgresql database

You can install Postgresql in two diffrenet ways, you can install there GUI App or a terminal Package with homebrew.

### GUI App installation ***preferred***

- Go to <https://postgresapp.com/downloads.html> and download the lateset version.

- Install the app

## Now lets create our first project

1. Go to Documents

``` bash
 cd Documents
```

2. Create a project folder

``` bash
 mkdir testdjango 
```

3. Go into the folder

``` bash
 cd testdjango
```

4. Install virtual inviroment

``` bash
 python3 -m venv venv
```

5. run the virtual inviroment

``` bash
 source venv/bin/activate
```

6. Install django

``` bash
 pip3 install django
```

7. Create django project

``` bash
django-admin startproject PROJECTNAME
```

***now youll notice a folder called 'app' and 'venv' we need to change the app folder name to out projects name***

8. Rename the app folder

``` bash
 mv app PROJECTNAME
```

9. Go into the project

``` bash
 cd PROJECTNAME
```

***Now you'll see the main app folder and a manage.py file***

***To start the project we need to change the database settings to pstgresql since django comes defult with sqlite3***

10. Install postgres module

``` bash
 pip install psycopg2
```

11. Changing django database settings

``` bash
 open PROJECTNAME/settings.py
```

12. Change the DATABASE section to the following and change the **DBNAME**

``` bash
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql_psycopg2',
        'NAME': "DBNAME",
        'USER': "postgres",
        'PASSWORD': "",
        'HOST': "127.0.0.1",
        'PORT': "5432",
    }
}
```

13. Open postgres application an Click on start


14. Click on the database icon that says "postgres"


15. In the new terminal window create your databse with the name that you typed in the settings file.

``` bash
 CREATE DATABASE DBNAME;
```

16. Go back to project terminal and migrate your database

``` bash
 ./manage.py migrate
```

17. Start Your project 

``` bash 
 ./manage.py runserver
```

18. Open your browser and enter the following ip

``` ip
127.0.0.1:8000
```

### Thats it!

### We are done.


## Additional command for django


- Create an app inside your project

``` bash 
 ./manage.py startapp APPNAME
```

- Create django super-user "admin"

``` bash
 ./manage.py createsuperuser
```
