# Name:NaveenKumar.T
# Reg No:212223220067
## Date: 28:02:2024
# Ex02 Django ORM Web Application
 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![entity relationship-1](https://github.com/820NaveenKumar208/ORM/assets/154746066/a393bbc3-c1be-4415-a69a-3153db2b8564)




## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM

### models.py
```
models.py

from django.db import models
from django.contrib import admin
class Book_DB(models.Model):
      sno=models.IntegerField(primary_key="sno");
      name=models.CharField(max_length=50);
      author=models.CharField(max_length=70);
      price=models.IntegerField();
      publisher=models.CharField(max_length=60);

class Book_DBAdmin(admin.ModelAdmin):
    list_display=("sno","name","author","price","publisher");
```
admin
```
from django.contrib import admin
from .models import Book_DB,Book_DBAdmin
admin.site.register(Book_DB,Book_DBAdmin)
```
## OUTPUT
![Screenshot (1)-1](https://github.com/820NaveenKumar208/ORM/assets/154746066/aea78f4a-3704-4518-a3b9-f7a603429eae)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
	
