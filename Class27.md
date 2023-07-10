# Reading Questions

## Explain the purpose and basic structure of Django models. How do they help in creating and managing database schema in a Django application?

Django web applications access and manage data through Python objects referred to as models. Models define the structure of stored data, including the field types and possibly also their maximum size, default values, selection list options, help text for documentation, label text for forms, etc. The definition of the model is independent of the underlying database — you can choose one of several as part of your project settings. Once you've chosen what database you want to use, you don't need to talk to it directly at all — you just write your model structure and other code, and Django handles all the dirty work of communicating with the database for you.


```python
from django.db import models

class Person(models.Model):
    first_name = models.CharField(max_length=30)
    last_name = models.CharField(max_length=30) 
```


## Describe the primary features and functionality of the Django Admin interface. How can it be customized to suit the specific needs of a project?


One of the most powerful parts of Django is the automatic admin interface. It reads metadata from your models to provide a quick, model-centric interface where trusted users can manage content on your site. The admin's recommended use is limited to an organization's internal management tool

## Briefly outline the key components and workflow of a Django application, as discussed in the Beginner’s Guide to Django. How do these components interact with each other to create a functional web application?                                                              

                                                                                   Django gets user requests by URL locator and responds back to it. django. urls module is used by it to manage the URL's requests. For any application in Django we create Python Module named as URLconf(URL configuration) as per Django Documentation.
