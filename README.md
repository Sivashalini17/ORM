# Ex01 Django ORM Web Application
# Date:10/05/2026

NAME : SIVA SHALINI.S
REG.NO : 212224240154

# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 cars

# PROGRAM

ADMIN.PY
```
from django.contrib import admin 
from .models import Car_Inventory, Car_InventoryAdmin 
admin.site.register(Car_Inventory, Car_InventoryAdmin)
```
MODELS.PY
```
from django.db import models 
from django.contrib import admin 

class  Car_Inventory(models.Model): 
    Car_Model = models.CharField()
    Engine_Type = models.CharField() 
    Car_Type = models.CharField() 
    Date = models.DateField()
    Car_Mileage = models.IntegerField()  
    

class Car_InventoryAdmin(admin.ModelAdmin): 
    list_display = ('Car_Model', 'Engine_Type', 'Car_Type', 'Date', 'Car_Mileage')
```

# OUTPUT

<img width="1488" height="805" alt="image" src="https://github.com/user-attachments/assets/74ef8d04-2a48-4128-bbe4-42c841eb8c2a" />

<img width="1910" height="965" alt="image" src="https://github.com/user-attachments/assets/f481d7d7-9bd9-4263-ae21-4b2a6798f9b9" />

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
