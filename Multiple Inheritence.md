# Arithmetic Operations Using Multiple Inheritance in Python

This Python program demonstrates **multiple inheritance** by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes.

## 🎯 Aim :

To write a Python program to calculate **Add, Sub & Division** using **Multiple Inheritance**.

## 🧠 Algorithm :

1. **Define `Calculation1` class**
   - Contains `Summation(a, b)` method to return the sum of two numbers.
2. **Define `Calculation2` class**
   - Contains `Subtraction(a, b)` method to return the difference of two numbers.
3. **Define `Derived` class**
   - Inherits from both `Calculation1` and `Calculation2`.
   - Contains `Division(a, b)` method to return the division result.
4. **Input**
   - Prompt the user to enter two numbers.
5. **Process**
   - Create an object of the `Derived` class.
   - Call `Summation`, `Subtraction`, and `Division` methods.
6. **Output**
   - Display the results of the three operations.

## 💻 Program :

class Add:

    def addition(self, a, b):
        print("Addition:", a + b)

class Sub:

    def subtraction(self, a, b):
        print("Subtraction:", a - b)

class Div:

    def division(self, a, b):
        print("Division:", a / b)

class Result(Add, Sub, Div):

    def get_values(self):
        self.a = int(input("Enter first number: "))
        self.b = int(input("Enter second number: "))

    def display(self):
        self.addition(self.a, self.b)
        self.subtraction(self.a, self.b)
        self.division(self.a, self.b)

obj = Result()

obj.get_values()

obj.display()

## Output Example :
<img width="241" height="127" alt="image" src="https://github.com/user-attachments/assets/58d9f13c-75e3-4fc8-8a09-30b13208968d" />

Result :
Thus the program is obtained and the output is obtained.



