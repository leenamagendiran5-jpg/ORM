# Ex02 Django ORM Web Application
## Date: 08.10.25

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
admin.py

from django.contrib import admin
from.models import Car,CarAdmin
admin.site.register(Car,CarAdmin)

models.py

from django.db import models
from django.contrib import admin
class Car(models.Model):
    car_name= models.CharField()
    car_model = models.CharField()
    release_date = models.DateField()
    millage = models.IntegerField()
    color = models.CharField()

class CarAdmin(admin.ModelAdmin):
    list_display = ('car_name', 'car_model', 'release_date', 'millage', 'color')
```
## OUTPUT

<img width="1556" height="858" alt="{3E6DEA53-31DF-4076-B8D5-2D2098276EB7}" src="https://github.com/user-attachments/assets/f3691846-cfe9-4fd6-836f-cfe3a280e439" />



## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
