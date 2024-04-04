# Ex02 Django ORM Web Application
## Date:04/04/24

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![ER-Diagram-Examples-5](https://github.com/selvasachein/ORM/assets/131433133/c5a90d83-c9e0-4f3b-ac94-068448eb9512)


## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM:
## models.py
```
from django.db import models
from django.contrib import admin
class Employee(models.Model):
    empid=models.IntegerField()
    empname=models.CharField(max_length=20)
    dept=models.CharField(max_length=10)
    salary=models.FloatField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('empid','empname','dept','salary')
```
## admin.py:
from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

## OUTPUT
![Screenshot (131)](https://github.com/selvasachein/ORM/assets/131433133/99baacba-9001-441e-86ed-7716090ec494)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
