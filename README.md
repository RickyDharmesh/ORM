# Ex02 Django ORM Web Application
# Date:26/09/2025
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
```
admin.py

from django.contrib import admin
from .models import car,car_Admin
admin.site.register(car,car_Admin)


models.py

from django.db import models
from django.contrib import admin 

class car(models.Model):
    Plate_No=models.CharField(max_length=15,primary_key=True)
    Name=models.CharField(max_length=10)
    Car_type=models.CharField(max_length=15)
    Date=models.IntegerField()
    Engine_type=models.CharField(max_length=10)

class car_Admin(admin.ModelAdmin):
    list_display=('Plate_No','Car_type','Date','Engine_type')  


# OUTPUT
![alt text](<Screenshot 2025-09-26 133510.png>)

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
