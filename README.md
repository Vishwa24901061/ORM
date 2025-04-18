# Ex02 Django ORM Web Application
## Date: 15/04/2025
## Name: VISHWA V
## Registor Number: 212224110062

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
```
from django.contrib import admin
from .models import Movie,MovieAdmin
admin.site.register(Movie,MovieAdmin)

from django.db import models
from django.contrib import admin
class Movie(models.Model):
    mid=models.IntegerField()
    mname=models.CharField(max_length=100)
    collection=models.IntegerField()
    year=models.IntegerField()
    rating=models.FloatField()

class MovieAdmin(admin.ModelAdmin):
    list_display=('mid','mname','collection','year','rating')
```

## OUTPUT

![Screenshot 2025-04-11 145144](https://github.com/user-attachments/assets/e4ca7d33-69a3-4e98-824e-a4fab7e0684a)

## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
