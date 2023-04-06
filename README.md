# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

## STEP 1:
Clone the problem from github

## STEP 2:
create a new app

## STEP 3:
Enter the codefor admin.py and model.py

## Step 4:
Execute Django admin and create 10 employees

Write your own steps

## PROGRAM
Model.py

from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.CharField(max_length=20,help_text="Employee ID")
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')  

Admin.py 
from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

## OUTPUT:
![emp](https://user-images.githubusercontent.com/118889143/230270168-12ee51ee-3c7b-407f-9f97-31ca38cf16d9.png)

## RESULT:
Thus a Django application to store and retrieve data from a database using Object Relational Mapping(ORM) is developed.
