# Django Models


## Overview

Models define the structure of stored data, including the field types and possibly also their maximum size, default values, selection list options, help text for documentation, label text for forms, etc.Once you've chosen what database you want to use, you don't need to talk to it directly at all — you just write your model structure and other code, and Django handles all the dirty work of communicating with the database for you.


### Fields

* The most important part of a model – and the only required part of a model – is the list of database fields it defines.

## Model primer

  1- Model definition: `models.py`

  2- Fields: ` my_field_name = models.CharField(max_length=20, help_text='Enter field documentation')`

  3- Metadata:
    ```
     class Meta:
        ordering = ['-my_field_name']
    ```

## Defining the LocalLibrary Models

* `from django.db import models`

## Re-run the database migrations

  ```
  python3 manage.py makemigrations
  python3 manage.py migrate
  ```


# Django Admin

## Overview:


The Django admin application can use your models to automatically build a site area that you can use to create, view, update, and delete records. This can save you a lot of time during development, making it very easy to test your models and get a feel for whether you have the right data. The admin application can also be useful for managing data in production, depending on the type of website.

## Registering models 

* First, open admin.py in the catalog application (`/locallibrary/catalog/admin.py`).

## Creating a superuser

`python3 manage.py createsuperuser`

## Bookmarks
- [Getting started with Django](https://docs.djangoproject.com/en/4.1/ref/models/fields/)

- [Django Tutorial Part 4: Django admin site](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Admin_site)
