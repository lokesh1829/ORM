# Ex01 Django ORM Web Application
## Date: 24/11/25

## AIM
To develop a Django application to store and retrieve data from a Car Inventory Database using Object Relational Mapping(ORM).

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
module.py 
'''from django.db import models
from django.contrib import admin
class car (models.Model):
    owner = models.CharField(max_length=100)
    make = models.CharField(max_length=100)
    model = models.CharField(max_length=100)
    year = models.IntegerField()

class carAdmin (admin.ModelAdmin):
    list_display = ('owner', 'make', 'model', 'year')'''

  admin.py
  '''from django.contrib import admin
from .models import car,carAdmin
admin.site.register(car, carAdmin)
'''



## OUTPUT
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/d27247aa-defc-48a9-9cbd-2d5356c8c09d" />



## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
