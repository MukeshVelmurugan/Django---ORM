# Django ORM Web Application

## AIM:
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram:
![image](https://user-images.githubusercontent.com/118707363/211722721-13618c86-9bec-4bb5-bfa2-ca4744196fac.png)


## DESIGN STEPS:

### STEP 1:
creating a table using meanings full details in ORM

### STEP 2:
upload the python code

### STEP 3:

push the code to github

## PROGRAM:
``` 
admin.py:

from django.contrib import admin
from .models import book,bookAdmin

admin.site.register(book,bookAdmin)

models.py

from django.db import models
from django.contrib import admin
# Create your models here.
class book(models.Model):
    book_id=models.CharField(primary_key=True,max_length=4,help_text='bookid')
    Authorname=models.CharField(max_length=50)
    Title=models.CharField(max_length=100)
    YearOfPublication=models.IntegerField()
    Price=models.IntegerField()
    

class bookAdmin(admin.ModelAdmin):
    list_display=('book_id','Authorname','Title','YearOfPublication','Price',)

```
## OUTPUT:
![image](https://user-images.githubusercontent.com/118707363/211722793-21c9ef39-7b8f-4a75-9520-66dbc9096e39.png)



## RESULT:
The code is executed successfully.

