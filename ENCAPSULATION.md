# Exp.No:29  
## Encapsulation

---

### AIM  
To write a Python program that defines a class Employee with a public method show() to display the details of an employee.

---

### ALGORITHM

1. Start the Program.
   
2. Define a class Employee.
3.Inside the class, define the __init__() method to initialize:
          
        -name
   
        -emp_id
   
        -designation
   
4.Define a public method show() to display the employee's name, ID, and designation.

5.Create an object of the Employee class with sample data.

6.Call the show() method to display the employee's details.

7.End the program.

---

### PROGRAM
Reg no: 212223020023
Name: Shanthosh S
```

class Student:
    def __init__(self, name, age):
        self.__name = name
        self.__age = age

    # Getter for age
    @property
    def age(self):
        return self.__age

    # Setter for age
    @age.setter
    def age(self, age):
        if age > 0 and isinstance(age, int):
            self.__age = age
        else:
            print("Please enter a valid age")

    # Method to print student details
    def print_details(self):
        return f"Name: {self.__name} {self.__age}"

# Create an instance
s = Student(" Jessa Salary:", 10000)
print(s.print_details())
# Change age using setter
s.age = 10000
print(s.print_details())



```

### OUTPUT
![Screenshot 2025-04-28 210408](https://github.com/user-attachments/assets/c8694416-d90b-4d7f-9f8e-d2a1c49c3066)


### RESULT
The program successfully creates an Employee class and uses a public method show() to display the details of the employee.


