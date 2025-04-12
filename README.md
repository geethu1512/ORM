# Ex02 Django ORM Web Application
## Name: GEETHU R
## Register No. :212224040089
## Date: 12-04-2025

## AIM
To develop a Django application to store and retrieve data from Movies Database using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 6 movie names

## PROGRAM
~~~
models.py

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


admin.py

from django.contrib import admin
from .models import Movie,MovieAdmin
admin.site.register(Movie,MovieAdmin)
~~~
## OUTPUT


![Screenshot 2025-04-12 143820](https://github.com/user-attachments/assets/357c3740-d4d3-44cb-961a-f97df96f959c)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully.
