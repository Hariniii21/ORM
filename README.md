# Ex02 Django ORM Web Application
## Date: 18.03.2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![er diagram](https://github.com/Hariniii21/ORM/assets/147140423/de2b76e0-ece6-4693-baf6-a6e9aadd7f69)


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
```
models.py
from django.db import models
from django.contrib import admin
class BookDetails(models.Model):
   student_name=models.CharField(max_length=20);
   id_no=models.IntegerField();
   email=models.EmailField();
   BookName=models.CharField(max_length=100,primary_key="True");
   author_name=models.CharField(max_length=20);
   Total_page=models.IntegerField();

class BookDetailsAdmin(admin.ModelAdmin):
  list_display=("student_name","id_no","email","BookName","author_name","Total_page")


admin.py
from django.contrib import admin
from .models import BookDetails,BookDetailsAdmin
admin.site.register(BookDetails,BookDetailsAdmin)
```

## OUTPUT
![Screenshot 2024-02-28 093442](https://github.com/Hariniii21/ORM/assets/147140423/f21b7c0e-665b-430d-ba05-db516e0fc57c)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
