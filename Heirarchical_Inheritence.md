# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

## 🧠 Algorithm

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program
~~~
class Details:
    def get_details(self,id1,name,gender):
        self.id1 = id1
        self.name = name
        self.gender = gender
        
class Employee(Details):
    def em_details(self,company,edep):
        self.company = company
        self.edep = edep
    def em_display(self):
        print("Employee Object")
        print("Id: ",self.id1)
        print("Name: ",self.name)
        print("Gender: ",self.gender)
        print("Company: ",self.company)
        print("Department: ",self.edep)

class Patient(Details):
    def py_details(self,hospital,pdep):
        self.hospital = hospital
        self.pdep = pdep
    def py_display(self):
        print("\nPatient Object")
        print("Id: ",self.id1)
        print("Name: ",self.name)
        print("Gender: ",self.gender)
        print("Hospital: ",self.hospital)
        print("Department: ",self.pdep)

eid1 = int(input())
ename = input()
egender = input()
company = input()
edep = input()

pid1 = int(input())
pname = input()
pgender = input()
hospital = input()
pdep = input()

e = Employee()
e.get_details(eid1,ename,egender)
e.em_details(company,edep)
e.em_display()

p = Patient()
p.get_details(pid1,pname,pgender)
p.py_details(hospital,pdep)
p.py_display()
        
~~~
## Sample Output
<img width="514" height="458" alt="{F1500627-59CA-49AD-ADC6-0F229F8DB15C}" src="https://github.com/user-attachments/assets/f22cacb7-40fd-4ddc-8dc4-0d32b3d2a016" />

