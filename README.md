# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![ent](https://github.com/Adchayakiruthika/django-orm-app/assets/138849219/33490d5c-f8b2-4ffe-be52-4ffc798483ad)



## DESIGN STEPS

### STEP 1:
creating a table using required details in Django-ORM

### STEP 2:
upload the python code.

### STEP 3:
push the code to github

## PROGRAM
```html
from django.db import models
from django.contrib import admin

# Create your models here.
class Student (models.Model):
    referencenumber=models.CharField(primary_key=True,max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()
    number=models.IntegerField()
class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email','number')
    ```

### admin.py
```html
from django.contrib import admin
from .models import Student,StudentAdmin

admin.site.register(Student,StudentAdmin)
```

## OUTPUT
![out1](https://github.com/Adchayakiruthika/django-orm-app/assets/138849219/b986abef-31c0-4fdc-a311-3e20f730621e)
![out2](https://github.com/Adchayakiruthika/django-orm-app/assets/138849219/913f8a3e-56b3-4fc6-a338-bfcd6bc5ec13)

## RESULT
The above program is executed successfully.
