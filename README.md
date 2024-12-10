# Ex02 Django ORM Web Application
# Date:
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
model.py
from django.db import models
from django.contrib import admin
class Bankloan (models.Model):
     acc=models.IntegerField(primary_key="acc")
     name=models.CharField(max_length=100)
     mobileno=models.IntegerField()
     pancode=models.IntegerField()
     aadharcode=models.IntegerField()
     
class BankloanAdmin(admin.ModelAdmin):
  list_display=('acc','name','mobileno','pancode','aadharcode')

admin.py
from django.contrib import admin
from .models import Bankloan,BankloanAdmin
admin.site.register(Bankloan,BankloanAdmin)
```

# OUTPUT
![alt text](<Screenshot 2024-12-07 194148.png>)
![alt text](<Screenshot 2024-12-07 194202.png>)
![alt text](<Screenshot 2024-12-10 134745.png>)
# RESULT
Thus the program for creating a database using ORM hass been executed successfully
