# Exp.No:28  
## Abstraction

---

### AIM  
To write a Python program that demonstrates the concept of abstract classes using a base class VEHICLE with two unimplemented (abstract) methods, which are implemented in the child classes CAR and BIKE.

---

### ALGORITHM

1.Start.

2.Import the ABC and abstractmethod decorators from Python’s abc module.

3.Create an abstract class VEHICLE.

4.Define two abstract methods: start() and stop().

5.Create a child class CAR that inherits from VEHICLE.

6.Implement the start() and stop() methods.

7.Create another child class BIKE that also inherits from VEHICLE.

8.Implement the start() and stop() methods.

9.Create objects of both CAR and BIKE and call their methods.

10.End


---

### PROGRAM
Reg no: 212223020023
Name: Shanthosh S

```
from abc import ABC, abstractmethod

class Vehicle(ABC):
    @abstractmethod
    def start(self):
        pass

    @abstractmethod
    def stop(self):
        pass

class Bike(Vehicle):
    def start(self):
        return "Bike is Started"

    def stop(self):
        return "Bike is stopped"

    def accelerate(self):
        return "Bike is accelrating @ 60kmph"

    def park(self):
        return "Bike is parked at two wheeler parking"

class Car(Vehicle):
    def start(self):
        return "Car is Started"

    def stop(self):
        return "Car is stopped"

    def accelerate(self):
        return "Car is accelrating @ 90kmph"

    def park(self):
        return "Car is parked at four wheeler parking"

# Create instances
bike = Bike()
car = Car()

# Invoke the methods
print("Bike Object")
print(bike.start())
print(bike.accelerate())
print(bike.park())
print(bike.stop())

print("\nCar Object")
print(car.start())
print(car.accelerate())
print(car.park())
print(car.stop())


```

### OUTPUT
![Screenshot 2025-04-28 210818](https://github.com/user-attachments/assets/7511df4d-81fb-4221-a821-a1cd79ac772d)



### RESULT
The program successfully demonstrates the use of an abstract base class (VEHICLE) with two abstract methods (start() and stop()), which are implemented in the derived classes CAR and BIKE. Upon execution, the program correctly displays start and stop messages for both car and bike.
