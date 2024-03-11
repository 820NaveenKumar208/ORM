# Develop By:Naveen Kumar.T
# reg No: 212223220067
# Ex02 Django ORM Web Application
## Date: 02/02/2024

## AIM:
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram:
![WhatsApp Image 2024-03-05 at 05 49 39_3bc3069b](https://github.com/selvasachein/ORM/assets/154746066/a0901127-495a-4306-b4f4-b13396545bd3)



## DESIGN STEPS:

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
	author=models.CharField(max_length=20);
	book_name=models.CharField(max_length=50);
	book_no=models.CharField(primary_key="book_no",max_length=10);
	customer_id=models.CharField(max_length=20);
	edition_year=models.IntegerField();
	shelfno=models.CharField(max_length=20);
	

class Book_DBAdmin(admin.ModelAdmin):
	list_display=("author","book_name","book_no","customer_id");
```
### admin.py
```
from django.contrib import admin
from .models import Book_DB,Book_DBAdmin
admin.site.register(Book_DB,Book_DBAdmin)
```

## OUTPUT

![Screenshot (69)](https://github.com/selvasachein/ORM/assets/154746066/51a00db9-3036-45dd-b351-c4195a141ffb)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
