# Multilevel Inheritance Example in Python

This Python project demonstrates the concept of **Multilevel Inheritance** to collect and display the **name**, **age**, and **location** of a person.

## 🎯 Aim :

To write a Python program that uses multilevel inheritance to get and display a person’s name, age, and location.

## 🧠 Algorithm :

1. **Parent Class**  
   - `__init__(name)` initializes the `name` attribute.  
   - `getName()` returns the `name`.

2. **Child Class (inherits Parent)**  
   - `__init__(name, age)` initializes `name` using `super()` and adds `age`.  
   - `getAge()` returns the `age`.

3. **Grandchild Class (inherits Child)**  
   - `__init__(name, age, location)` initializes `name` and `age` using `super()` and adds `location`.  
   - `getLocation()` returns the `location`.

4. **Input & Output**  
   - Take user input for name, age, and location.  
   - Create an instance of `Grandchild`.  
   - Print all details using class methods.

## Program :

class Person:

    def get_name(self):
        self.name = input("Enter name: ")

class Age(Person):

    def get_age(self):
        self.age = int(input("Enter age: "))

class Location(Age):

    def get_location(self):
        self.location = input("Enter location: ")

    def display(self):
        print("Name:", self.name)
        print("Age:", self.age)
        print("Location:", self.location)

obj = Location()

obj.get_name()

obj.get_age()

obj.get_location()

obj.display()

## Sample Output :
<img width="212" height="156" alt="image" src="https://github.com/user-attachments/assets/90b17658-7e6e-40ed-8a2f-34384f884c04" />

Result :

Thus the program is excuted and the output is obtained .
