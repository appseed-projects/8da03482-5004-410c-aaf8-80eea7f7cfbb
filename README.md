# Django Soft Dashboard

Open-source **Django Dashboard** generated by `AppSeed` op top of a modern design. Designed for those who like bold elements and beautiful websites, **[Soft UI Dashboard](https://appseed.us/generator/soft-ui-dashboard/)** is ready to help you create stunning websites and webapps. **Soft UI Dashboard** is built with over 70 frontend individual elements, like buttons, inputs, navbars, nav tabs, cards, or alerts, giving you the freedom of choosing and combining.

<br />

> Context:

- Built with [Soft UI Dashboard Generator](https://appseed.us/generator/soft-ui-dashboard/)
- Timestamp: `2022-05-08 10:54`
- Build ID: `8da03482-5004-410c-aaf8-80eea7f7cfbb`

<br />

> 👉 **Free [Support](https://appseed.us/support/)** (registered users) via `Email` and `Discord`

<br />

## ✨ Features

- `Up-to-date dependencies`
- UI-Ready app, `SQLite Database`, Django Native ORM
- `Session-Based authentication`, Forms validation

<br />


## ✨ Start the app in Docker

> `Note`: Make sure you are in the root of the project. 

```bash
$ docker-compose up --build 
```

Visit `http://localhost:85` in your browser. The app should be up & running.

<br />


![Django Soft UI Dashboard - Seed project generated by AppSeed.](https://user-images.githubusercontent.com/51070104/119937082-d5524080-bf92-11eb-83b2-19034824e934.png)

<br />

## ✨ How to use it

> Download the code 

```bash
$ # Get the code
$ git clone https://github.com/appseed-projects/8da03482-5004-410c-aaf8-80eea7f7cfbb.git
$ cd 8da03482-5004-410c-aaf8-80eea7f7cfbb
```

<br />

### 👉 Set Up for `Unix`, `MacOS` 

> Install modules via `VENV`  

```bash
$ virtualenv env
$ source env/bin/activate
$ pip3 install -r requirements.txt
```

<br />

> Set Up Database

```bash
$ python manage.py makemigrations
$ python manage.py migrate
```

<br />

> Start the app

```bash
$ python manage.py runserver
```

At this point, the app runs at `http://127.0.0.1:8000/`. 

<br />

### 👉 Set Up for `Windows` 

> Install modules via `VENV` (windows) 

```
$ virtualenv env
$ .\env\Scripts\activate
$ pip3 install -r requirements.txt
```

<br />

> Set Up Database

```bash
$ python manage.py makemigrations
$ python manage.py migrate
```

<br />

> Start the app

```bash
$ python manage.py runserver
```

At this point, the app runs at `http://127.0.0.1:8000/`. 

<br />

## ✨ Create Users

By default, the app redirects guest users to authenticate. In order to access the private pages, follow this set up: 

- Start the app via `flask run`
- Access the `registration` page and create a new user:
  - `http://127.0.0.1:8000/register/`
- Access the `sign in` page and authenticate
  - `http://127.0.0.1:8000/login/`

<br />

## ✨ Code-base structure

The project is coded using a simple and intuitive structure presented below:

```bash
< PROJECT ROOT >
   |
   |-- core/                               # Implements app configuration
   |    |-- settings.py                    # Defines Global Settings
   |    |-- wsgi.py                        # Start the app in production
   |    |-- urls.py                        # Define URLs served by all apps/nodes
   |
   |-- apps/
   |    |
   |    |-- home/                          # A simple app that serve HTML files
   |    |    |-- views.py                  # Serve HTML pages for authenticated users
   |    |    |-- urls.py                   # Define some super simple routes  
   |    |
   |    |-- authentication/                # Handles auth routes (login and register)
   |    |    |-- urls.py                   # Define authentication routes  
   |    |    |-- views.py                  # Handles login and registration  
   |    |    |-- forms.py                  # Define auth forms (login and register) 
   |    |
   |    |-- static/
   |    |    |-- <css, JS, images>         # CSS files, Javascripts files
   |    |
   |    |-- templates/                     # Templates used to render pages
   |         |-- includes/                 # HTML chunks and components
   |         |    |-- navigation.html      # Top menu component
   |         |    |-- sidebar.html         # Sidebar component
   |         |    |-- footer.html          # App Footer
   |         |    |-- scripts.html         # Scripts common to all pages
   |         |
   |         |-- layouts/                   # Master pages
   |         |    |-- base-fullscreen.html  # Used by Authentication pages
   |         |    |-- base.html             # Used by common pages
   |         |
   |         |-- accounts/                  # Authentication pages
   |         |    |-- login.html            # Login page
   |         |    |-- register.html         # Register page
   |         |
   |         |-- home/                      # UI Kit Pages
   |              |-- index.html            # Index page
   |              |-- 404-page.html         # 404 page
   |              |-- *.html                # All other pages
   |
   |-- requirements.txt                     # Development modules - SQLite storage
   |
   |-- .env                                 # Inject Configuration via Environment
   |-- manage.py                            # Start the app - Django default start script
   |
   |-- ************************************************************************
```

<br />

---
Django Soft Dashboard - Open-source starter generated by **[AppSeed Generator](https://appseed.us/generator/)**.
