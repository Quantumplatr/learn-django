# Learn Django

## Table of Contents
- [Learn Django](#learn-django)
  - [Table of Contents](#table-of-contents)
  - [1. Setup](#1-setup)
    - [1.1 Install Django](#11-install-django)
    - [1.2 Creating a Project](#12-creating-a-project)
    - [1.3 Running the Server](#13-running-the-server)
  - [2. Development](#2-development)
  - [3. Testing](#3-testing)
  - [Resources](#resources)

## 1. Setup
### 1.1 Install Django
[This](https://docs.djangoproject.com/en/4.0/topics/install/) is a detailed tutorial. [Here](https://docs.djangoproject.com/en/4.0/intro/install/) is the quick version.

Make sure you have python. You can check your version with:
```bash
$ python --version
```

For database work, [install a db](https://docs.djangoproject.com/en/4.0/topics/install/#database-installation).

Install Django with pip:
```bash
$ python -m pip install Django
```

Verify Django is installed:
```bash
$ python
>>> import django
>>> print(django.get_version())
4.0.2
>>> quit()
```
or
```bash
$ python -m django --version
```

### 1.2 Creating a Project
`cd` into the desired directory. Run teh following command:

```bash
$ django-admin startproject <project-name>
```

This generates this file structure:
```
<project-name>/
    manage.py
    <project-name>/
        __init__.py
        settings.py
        urls.py
        asgi.py
        wsgi.py
```

In order these are:
- `<project-name>/`: Container folder that you can rename if desired
- `manage.py`: Command-line utility for managing the project (see [this](https://docs.djangoproject.com/en/4.0/ref/django-admin/))
- `<project-name>/`: The Python package for this project. This folder name is used for imports (e.g. `<project-name>.urls`)
- `__init__.py`: Empty file telling Python that this is a package
- `settings.py`: Project config/settings (see [this](https://docs.djangoproject.com/en/4.0/topics/settings/))
- `urls.py`: URL declarations for the project. Like a table of contents. (see [this](https://docs.djangoproject.com/en/4.0/topics/http/urls/))
- `asgi.py`: "An entry-point for ASGI-compatible web servers to serve your project." (see [this](https://docs.djangoproject.com/en/4.0/howto/deployment/asgi/))
- `wsgi.py`: "An entry-point for WSGI-compatible web servers to serve your project." (see [this](https://docs.djangoproject.com/en/4.0/howto/deployment/wsgi/))

### 1.3 Running the Server
Run the server by `cd`ing into the container `<project-name>` folder and running:
```bash
$ python manage.py runserver
```

TODO finish

## 2. Development

TODO 

## 3. Testing

TODO

## Resources
1. [Quick Django Install](https://docs.djangoproject.com/en/4.0/intro/install/)
2. [Django Install](https://docs.djangoproject.com/en/4.0/topics/install/)
3. [Django Tutorial (start)](https://docs.djangoproject.com/en/4.0/intro/tutorial01/)
4. [Django Project Management](https://docs.djangoproject.com/en/4.0/ref/django-admin/)
5. [Django Project Settings](https://docs.djangoproject.com/en/4.0/topics/settings/)
6. [Django URL Dispatcher](https://docs.djangoproject.com/en/4.0/topics/http/urls/)