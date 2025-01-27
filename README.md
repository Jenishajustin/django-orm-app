# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![erdiagram](https://user-images.githubusercontent.com/119405070/215317816-d76ac97f-a7a5-4c6a-bf73-d93cef6af260.png)
<br>

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

![ORMoutput](https://user-images.githubusercontent.com/119405070/210609659-f13972ed-f94c-423b-ad5b-5bbb40773b47.png)
<br>

![ORM](https://user-images.githubusercontent.com/119405070/210609751-d0f03828-670f-402b-ac19-c49b1a2a31ef.png)
<br>

## RESULT
The app is created and executed properly.
