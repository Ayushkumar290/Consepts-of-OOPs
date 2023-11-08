# OOPs Concepts in Python
* Class
  - A class is a set of specifications or blueprint about an entity. it definesa set of data element and methods also called as attributes and behaviors.   
~~~
    class Dog:  
        pass
~~~      
- Objects or Instance    
  The object is an entity that has a state and behavior associated with it.  
  to create an object we need special method called as **Constructor**  
  **Constructur** is a method inside a class having some special features  
    1. Same name as class name  
    2. No return type
    4. Used to initialize fields of an object  
  - **Creating an Object**      
    * Static Binding  
    * Dynamic Binding    
  **Static Binding**  - Compiler know about the memory occupied by an object  
  **Dynamic Binding** - Memory is allocated at run time using ***new*** keyword
* Example : **Static binding**  
~~~
public class StaticBindingExample {
public static void main(String args[]) {
Vehicle veh = new MotorBike();
veh.start();
}
}
class Vehicle {
static void start() {
System.out.println("vehicle will start now..");
}
}
class MotorBike extends Vehicle {
static void start() {
System.out.println("Bike will start now..");
}
}
~~~
**Dynamic Binding**
~~~
class Colony{
//method to start the electricity of the Colony
void startElectricity(){
//printing the message here
System.out.println("Colony Electricity is On.");
}
}
//Child class implementation
class Building extends Colony{
//method to start the electricity of Building
void startElectricity(){
//printing the message here
System.out.println("Building Electricity is On.");
}
}
public class StaticBindingExample {
public static void main(String args[]) {
//Creating object of the parent class type
Colony col = new Colony();
col.startElectricity();
//Creating object of the child class type
Colony col2 = new Building();
col2.startElectricity();
}
}
~~~
* Object in python
~~~
        obj = Dog()
~~~
* Python Self - Class methods must have an extra first parameter in the method definition. We do not give a value for this parameter when we call the method, Python provides it
If we have a method that takes no arguments, then we still have to have one argument.
This is similar to this pointer in C++ and this reference in Java.
Example :
~~~
# Creating Class
class Student:
    # Creating A sonstructor
    def __init__(self,name,cls,roll_no):
        self.name = name
        self.cls = cls
        self.roll_no = roll_no
    # Creating a funtion that print information of the person
    def info(self):
        print(f"Student's name is {self.name}, who studies in class {self.cls} and roll no {self.roll_no}")

# Creating an object
a = Student("lucky","BSC H CS",1351)

# Creating another object
b = Student("Aman","BSC H Maths", 3432)

# Calling info() from class
a.info()
b.info()

# Chainging the name of Student a
a.name = "mohit"
a.info()
~~~
* Reference - A reference is a name that refers to the specific location in memory of a value (object).
in python
~~~
a = 343
~~~

# Polymorphism  
-
# Encapsulation  
# Inheritance  
# Data Abstraction  
![](https://media.geeksforgeeks.org/wp-content/uploads/20230818181616/Types-of-OOPS-2.gif)  
