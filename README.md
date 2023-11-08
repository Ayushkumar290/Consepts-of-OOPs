# OOPs Concepts in Python
* Class
  - A class is a set of specifications or blueprint about an entity. it definesa set of data element and methods also called as attributes and behaviors.   
  * Classes are created by keyword class.   
  * Attributes are the variables that belong to a class.   
  * Attributes are always public and can be accessed using the dot (.) operator. Eg.: Myclass.Myattribute  
  * Example :Creating an Empty Class in Python
~~~
    class Dog:  
        pass
~~~      
* Objects or Instance    
  The object is an entity that has a state and behavior associated with it.  
* Creating an Object  
  * to create an object we need special method called as **Constructor**  
  **Constructur** is a method inside a class having some special features  
    1. Same name as class name  
    2. No return type  
    3. Used to initialize fields of an object  
**Creating an Object**      
    * Static Binding  
    * Dynamic Binding    
  **Static Binding**  - Compiler know about the memory occupied by an object  
  **Dynamic Binding** - Memory is allocated at run time using ***new*** keyword  
Example : **Static binding**  
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

~~~
        obj = Dog()
~~~
  * Python Self - 
* Reference
# Polymorphism  
# Encapsulation  
# Inheritance  
# Data Abstraction  
![](https://media.geeksforgeeks.org/wp-content/uploads/20230818181616/Types-of-OOPS-2.gif)  
