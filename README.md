# Ex02 Django ORM Web Application
## Date: 16/11/2024

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![alt text](<Screenshot 2024-12-10 110413.png>)


## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for a minimum of 5 userswho obtain loan from bank and create a minimum of 5 admin users

## PROGRAM
```
admin.py
from django.contrib import admin
from .models import Bank_loan,Bank_loanadmin
admin.site.register(Bank_loan,Bank_loanadmin)

models.py
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

Include the screenshot of your admin page.
![alt text](<Screenshot (4).png>)
![alt text](<Screenshot (5).png>)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
