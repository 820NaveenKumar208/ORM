# Ex02 Django ORM Web Application
## Date: 05.03.2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![Entity diagram](https://github.com/ARAVIND23005370/ORM/assets/154746066/459ae4ee-9c1c-4ab8-a47a-f8e0cbbe6195)

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
## models.py
```
from django.db import models
from django.contrib import admin
class Book_DB(models.Model):
	author=models.CharField(max_length=20);
	book_name=models.CharField(max_length=50);
	book_no=models.CharField(primary_key="book_no",max_length=10);
	customer_id=models.CharField(max_length=20);
	edition_year=models.IntegerField();
	shelfno=models.CharField(max_length=20);
class Book_DBAdmin(admin.ModelAdmin):
	list_display=("author","book_name","book_no","customer_id","edition_year","shelfno");
```
## admin.py
```
from django.contrib import admin
from .models import Book_DB,Book_DBAdmin
admin.site.register(Book_DB,Book_DBAdmin)
```
## OUTPUT

![Website Book link](https://github.com/ARAVIND23005370/ORM/assets/154746066/04bf362d-2342-4f87-8c93-4752dc2cfd29)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
