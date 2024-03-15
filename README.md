# Name:NaveenKumar.T
# Reg No:212223220067
## Date: 28:02:2024
# Ex02 Django ORM Web Application
 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![alt text](<WhatsApp Image 2024-03-05 at 05.49.40_68a739b3.jpg>)

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
from django.db import models
from django.contrib import admin
class Book_DB(models.Model):
	Author=models.CharField(max_length=20);
	Book_Name=models.CharField(max_length=50);
	book_No=models.CharField(primary_key="book_no",max_length=10);
	Customer_Id=models.CharField(max_length=20);
	

class Book_DBAdmin(admin.modelAdmin):
	list_display=("aAthor","Book_Name","Book_No","Customer_Id");
```
### admin.py
```
from django.contrib import admin
from .models import Book_DB,Book_DBAdmin
admin.site.register(Book_DB,Book_DBAdmin)

```
## OUTPUT

![alt text](<Screenshot (69).png>)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
	
