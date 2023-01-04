# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
To create a ORM-APP using our own webserver.
### STEP 2:
Execute the commands correctly in the terminal and make some changes in the models.py and admin.py and run the server.
### STEP 3:
Open the Django server and the app is ready to execute our informations.

## PROGRAM
```python
from django.db import models
from django.contrib import admin
## Create your models here.
class Employement(models.Model):
employementnumber=models.IntegerField(max_length=20,help_text="employementnumber")
employementname=models.CharField(max_length=100)
age=models.IntegerField()
email=models.EmailField()
place=models.CharField(max_length=20,help_text="place")
designation=models.CharField(max_length=20,help_text="designation")
salary=models.CharField()
class EmployementAdmin(admin.ModelAdmin):
list_display=('employementnumber','employementname','age','email','place','designation','salary')
```

## OUTPUT

Include the screenshot of your admin page.
![MODELS](ORMoutput.png)

![MODELS](ORM.png)
## RESULT
The app is created and executed properly.