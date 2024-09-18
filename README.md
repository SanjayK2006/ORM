# Ex 02 Django ORM Web Application
## DATE: 04-09-24

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create 10 Football players

## PROGRAM

```py
Models.py

from django.db import models
from django.contrib import admin
class Players(models.Model):
    jrsy=models.CharField(max_length=20,help_text="Player Jrsy")
    name=models.CharField(max_length=100)
    cntry=models.CharField(max_length=100)
    age=models.IntegerField()
    height=models.IntegerField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('jrsy','name','cntry','age','height')


Admin.py

from django.contrib import admin
from .models import Players,EmployeeAdmin
admin.site.register(Players,EmployeeAdmin)
```

## OUTPUT

![image](https://github.com/rahulramakrishnann/Exp-2-ORM--web/assets/143045415/b2e404af-f088-492e-b606-6ebffece8f02)
![image](https://github.com/rahulramakrishnann/Exp-2-ORM--web/assets/143045415/94c3d887-112e-4b9b-b83a-7365148fb61f)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
