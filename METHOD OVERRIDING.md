# Exp.No:26  
## Method Overriding

---

### AIM  
To write a Python program to create a Parent class `Bird` and inherit two child classes `Sparrow` and `Ostrich` from the `Bird` class with the same method `flight()`. Create an object for each class and call the methods of the class which will print the name of the bird that is flying.


---

### ALGORITHM

1. **Begin the program.**
2. **Define the Bird class**:
   - Create a method `intro()` to print "There are many types of birds."
   - Create a method `flight()` to print "Most of the birds can fly but some cannot."
3. **Define the Sparrow class**, which inherits from `Bird`:
   - Override the `flight()` method.
   - Call the `intro()` method from the parent class.
   - Print "Sparrows can fly."
4. **Define the Ostrich class**, which inherits from `Bird`:
   - Override the `flight()` method.
   - Call the `intro()` method from the parent class.
   - Print "Ostriches cannot fly."
5. **Create an object `obj_bird`** of the `Bird` class.
6. **Create an object `obj_spr`** of the `Sparrow` class.
7. **Create an object `obj_ost`** of the `Ostrich` class.
8. **Print the general message** "There are many types of birds."
9. **Call the `flight()` method** on each object (`obj_bird`, `obj_spr`, `obj_ost`) to display the respective messages.
10. **Terminate the program.**

---

### PROGRAM
Reg No: 212223020023
Name: Shanthosh S
```
# Parent class
class Bird:
    def flight(self):
        print("Most birds can fly.")

# Child class 1
class Sparrow(Bird):
    def flight(self):
        print("Sparrow is flying high in the sky!")

# Child class 2
class Ostrich(Bird):
    def flight(self):
        print("Ostrich cannot fly.")

# Creating objects
bird = Bird()
sparrow = Sparrow()
ostrich = Ostrich()

# Calling methods
print("Bird class:")
bird.flight()

print("\nSparrow class:")
sparrow.flight()

print("\nOstrich class:")
ostrich.flight()


```

### OUTPUT
![Screenshot 2025-04-28 211710](https://github.com/user-attachments/assets/a7baef74-6758-4b39-8be6-b27bfddc2da1)


### RESULT
The program demonstrates inheritance and method overriding and terminates the program successfully.
