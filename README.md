# Ex01 Django ORM Web Application
## Date: 

## AIM
To develop a Django Application to store and retrieve data from a E-Commerce Website Database for Amazon or Flipkart using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Detect changes and create migration files that describe how to modify the database schema

### STEP 5:
Execute the migration files and update the database schema to match your Django models

### STEP 6:
Create a superuser with full access rights to all models and data through the admin interface.

### STEP 7:
Apply the migration files of the created app to the database

### STEP 8:
Execute Django admin using localhost and create details for 10 entries

## PROGRAM

```
admin.py 

from django.contrib import admin
from .models import Car_Inventory, Car_InventoryAdmin
admin.site.register(Car_Inventory, Car_InventoryAdmin)

models.py

from django.db import models
from django.contrib import admin
class  Car_Inventory(models.Model):
    Plate_No = models.CharField(max_length=20, primary_key=True)
    Car_Manufacturer = models.CharField(max_length=15)
    Car_Model = models.CharField(max_length=100)
    Car_Color = models.CharField(max_length=20)
    Mileage = models.IntegerField( )

class Car_InventoryAdmin(admin.ModelAdmin):
    	list_display = ('Plate_No', 'Car_Manufacturer','Car_Model', 'Car_Color', 'Mileage')

```

## OUTPUT

![WhatsApp Image 2025-12-04 at 10 02 33 PM](https://github.com/user-attachments/assets/f557acfd-ae7f-4e83-8392-6cfaa8c27a46)


## RESULT
Thus the program for creating E-commerce website database using ORM hass been executed successfully
