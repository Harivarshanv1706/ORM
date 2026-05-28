# Ex01 Django ORM Web Application
# Date: 28/05/2026
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
```
admin.py 

from django.contrib import admin
from .models import Employee, EmployeeAdmin
admin.site.register(Employee, EmployeeAdmin)

models.py

from django.db import models
from django.contrib import admin

class Employee(models.Model):
    eid=models.CharField(max_length=20, help_text="Employee ID")
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')
```
# OUTPUT
<img width="1918" height="1198" alt="image" src="https://github.com/user-attachments/assets/d41c7476-0c58-427d-b48b-0846b4f66f5b" />

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
