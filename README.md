# django-tutorial-site

https://docs.djangoproject.com/en/3.1/intro/tutorial01/

https://docs.djangoproject.com/en/3.1/intro/tutorial02/

## Run locally
```
pipenv shell
pipenv install
python manage.py runserver
```

## Run tests for app

```
python manage.py test <app>
```

Example:
```
python manage.py test polls
```

## Where are default pages?

Run this:
```
python -c "import django; print(django.__path__)"
```

You will get the path, then drill down to PATH/contrib/admin/templates/admin/base_site.html, for example, to see the admin page.

You can copy that page into templates/admin directory and modify it!

> since APP_DIRS is set to True, Django automatically looks for a templates/ subdirectory within each application package, for use as a fallback (don’t forget that django.contrib.admin is an application).
