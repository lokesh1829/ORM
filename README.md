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
```
models.py
from django.db import models
from django.contrib import admin
class car (models.Model):
    owner = models.CharField(max_length=100)
    make = models.CharField(max_length=100)
    model = models.CharField(max_length=100)
    year = models.IntegerField()

class carAdmin (admin.ModelAdmin):
    list_display = ('owner', 'make', 'model', 'year')

```
```
admin.py
from django.contrib import admin
from .models import car,carAdmin
admin.site.register(car, carAdmin)

```



## OUTPUT
<img width="1920" height="1080" alt="Screenshot 2025-11-24 141658" src="https://github.com/user-attachments/assets/f4b139ce-1480-48b1-86fa-8319ee6b0cfd" />




## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
