# Ex02 Django ORM Web Application
# Date:19/10/2024
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
```python
models.py:
from django.db import models
from django.contrib import admin
class bankloan(models.Model):
    Name=models.CharField(max_length=100)
    Accountno=models.IntegerField(primary_key="Accountno")
    Startdate=models.DateField()
    Email=models.EmailField()
    Mobilenumber=models.IntegerField()
    Amount=models.IntegerField()

class bankloanAdmin(admin.ModelAdmin):
    list_display=('Name','Accountno','Startdate','Email','Mobilenumber','Amount')

admin.py:
from django.contrib import admin
from .models import bankloan,bankloanAdmin
admin.site.register(bankloan,bankloanAdmin)


```
# OUTPUT
![WhatsApp Image 2024-12-07 at 10 48 41 PM](https://github.com/user-attachments/assets/65e9e71a-6c8e-4da4-959e-715097a2981a)
![Screenshot 2024-12-07 230142](https://github.com/user-attachments/assets/683bf22c-6431-4c81-8910-44130767c515)
![Screenshot 2024-12-07 231534](https://github.com/user-attachments/assets/f57432de-9d52-4205-a53d-42f308f3b380)
![Screenshot 2024-12-12 132041](https://github.com/user-attachments/assets/68f66a55-7821-4813-bbf9-0c5bc21ea3fd)



# RESULT
Thus the program for creating a database using ORM hass been executed successfully
