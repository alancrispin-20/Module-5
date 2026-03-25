# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim :

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

## 🧠 Algorithm :

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program :
class Person:

    def get_data(self):
        self.name = input("Enter name: ")
        self.age = int(input("Enter age: "))

class Employee(Person):

    def get_employee(self):
        self.emp_id = input("Enter Employee ID: ")
        self.salary = input("Enter Salary: ")

    def display_employee(self):
        print("Employee Details")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Employee ID:", self.emp_id)
        print("Salary:", self.salary)

class Patient(Person):

    def get_patient(self):
        self.patient_id = input("Enter Patient ID: ")
        self.disease = input("Enter Disease: ")

    def display_patient(self):
        print("Patient Details")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Patient ID:", self.patient_id)
        print("Disease:", self.disease)

e = Employee()
e.get_data()
e.get_employee()
e.display_employee()

p = Patient()
p.get_data()
p.get_patient()
p.display_patient()

## Sample Output :
<img width="235" height="478" alt="image" src="https://github.com/user-attachments/assets/608e6d5b-8f6c-4d2b-a651-76ebfe6d9bb5" />

Result :
Thus the program is excuted and the output is obatined.


