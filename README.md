# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Enter the inputs
### STEP 2:
Make your codes
### STEP 3:
End the program

## PROGRAM
```
Admin.py
from django.contrib import admin
from .models import Student,StudentAdmin
# Register your models here.

admin.site.register(Student,StudentAdmin)
models.py
from django.db import models
from django.contrib import admin
# Create your models here.
class Student (models.Model):
    referencenumber=models.CharField(primary_key=True,max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()


class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email')
```

## OUTPUT
## SERVER OUTPUT:
![Screenshot (150)](https://user-images.githubusercontent.com/122793480/232839984-1fe174c1-0302-4deb-ad5c-3ee47644e993.png)

## CLIENT OUTPUT:
![Screenshot (151)](https://user-images.githubusercontent.com/122793480/232840005-39b55ffa-9373-495c-b19b-f488ac285735.png)


## RESULT
Thus the program executed successfully.
