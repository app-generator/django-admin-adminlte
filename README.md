# [Django AdminLTE Theme](https://github.com/app-generator/django-admin-adminlte)

Modern template for **Django Admin Interface** coded on top of **AdminLTE**, the iconic dashboard template.

> Actively supported by [AppSeed](https://appseed.us/) via `Email` and `Discord`.

<br>

**Links & Resources**

- UI Kit: [AdminLTE](https://github.com/ColorlibHQ/AdminLTE) `v3.2.0` by ColorLib
- [Django AdminLTE](https://adminlte-django.appseed-srv1.com/) - LIVE Demo

<br />

![AdminLTE - Full-Stack Starter generated by AppSeed.](https://user-images.githubusercontent.com/51070104/168842202-9b80a957-a375-4e6d-8247-2cc459267a86.png)

<br /> 

## Why `Django AdminLTE Theme`

- Modern `Bootstrap` Design
- `Responsive Interface`
- `Minimal Template` overriding
- `Easy integration`

<br />

## How to use it

<br />

> **Install the package** via `PIP` 

```bash
$ pip install django-admin-adminlte
// OR
$ pip install git+https://github.com/app-generator/django-admin-adminlte.git
```

<br />

> Add `admin_material` application to the `INSTALLED_APPS` setting of your Django project `settings.py` file (note it should be before `django.contrib.admin`):

```python
    INSTALLED_APPS = (
        ...
        'admin_material.apps.AdminLteDashboardConfig',
        'django.contrib.admin',
    )
```

<br />

> Add `LOGIN_REDIRECT_URL` and `EMAIL_BACKEND` of your Django project `settings.py` file:

```python
    LOGIN_REDIRECT_URL = '/'
    # EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
    EMAIL_BACKEND = 'django.core.mail.backends.console.EmailBackend'
```

<br />

> Add `admin_material` urls in your Django Project `urls.py` file

```python
    from django.urls import path, include

    urlpatterns = [
        ...
        path('', include('admin_adminlte.urls')),
    ]
```

<br />

> **Collect static** if you are in `production environment`:

```bash
$ python manage.py collectstatic
```

<br />

> **Start the app**

```bash
$ # Set up the database
$ python manage.py makemigrations
$ python manage.py migrate
$
$ # Create the superuser
$ python manage.py createsuperuser
$
$ # Start the application (development mode)
$ python manage.py runserver # default port 8000
```

Access the `admin` section in the browser: `http://127.0.0.1:8000/`

<br />

## Screenshots

@ToDo

<br />

---
**[Django AdminLTE Theme](https://github.com/app-generator/django-admin-adminlte)** - Modern Admin Interface provided by **[AppSeed](https://appseed.us/)**