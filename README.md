# Ex02 Django ORM Web Application
## Date:16/11/2024

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![image](https://github.com/user-attachments/assets/4183ed43-ada5-42dc-865c-4448f279441a)





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
ADMIN.Py
# Register your models here.
from django.contrib import admin
from .models import Bank_loan,Bank_loanadmin
admin.site.register(Bank_loan,Bank_loanadmin)

MODELS.PY

# Create your models here.
from django.db import models
from django.contrib import admin
class Bank_loan (models.Model):
    Customer_ID=models.CharField(max_length=20, primary_key=True)
    Customer_name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()
    loan_amt=models.IntegerField()
    DOB=models.DateField()
class Bank_loanadmin(admin.ModelAdmin):
    list_display=('Customer_ID','Customer_name','age','email','loan_amt','DOB')
```





## OUTPUT
![image](https://github.com/user-attachments/assets/e3225cc5-1d57-4a3c-8435-d7c2f891448f)
![image](https://github.com/user-attachments/assets/c4aae8e8-ddc1-4953-b5e0-8d503d416cee)



Include the screenshot of your admin page.


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
