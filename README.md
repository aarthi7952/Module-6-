## DATE: 22.10.2025

## AIM
To create an abstract class named Shape with an abstract method calculate_area, and implement this method in two subclasses: Rectangle and Circle.

## ALGORITHM
1.Import ABC module:
  Use from abc import ABC, abstractmethod to define abstract classes and methods.
2. Create Abstract Class Shape:
    Define an abstract method calculate_area() with @abstractmethod.
3.Create Subclass Rectangle:
    Set default values for length and breadth.
    Override calculate_area() to compute the rectangle area.
4.Create Subclass Circle:
    Set default value for radius.
    Override calculate_area() to compute the circle area.
5.Create Objects & Call Methods:
     Instantiate Rectangle and Circle.
     Call their calculate_area() methods.  

## Program
```
from abc import ABC
class Shape(ABC):
    def calculate_area(self):
        pass
class Rectangle(Shape):
    length = 5
    breadth =3 
    def calculate_area(self):
        return self.length * self.breadth

class Circle(Shape):
  radius = 4
  def calculate_area(self):
        return self.radius * self.radius*3.14

rec=Rectangle()
cir=Circle()#object created for the class 'Rectangle'
print("Area of a rectangle:", rec.calculate_area()) 
print("Area of a circle:", cir.calculate_area())
```
## OUTPUT
<img width="1177" height="271" alt="483894139-410a645c-1f20-4053-994e-521648c248e1" src="https://github.com/user-attachments/assets/71ed9c81-73ef-488f-9140-46288e61f10a" />

## RESULT
Thus, the python program has been executed successfully.

## Python OOP: Encapsulation with Private Members

## AIM
To implement Encapsulation in Python by defining a class Rectangle with private member variables __length and __breadth.

## ALGORITHM
1.Define the Class:
    Create a class Rectangle with two private attributes: __length and __breadth.
    
2.Initialize Variables:
    Use the init() constructor to set initial values for __length and __breadth.
    
3.Print Values:
    Display the private variables from within the class to demonstrate access.
    
4.Instantiate the Object:
     Create an object of the Rectangle class to trigger the constructor.
     
## Program
```
class Rectangle:
    def __init__(self, length, width):
        self.__length = length  # Private variable
        self.__width = width    # Private variable
    def print_values(self):
        print(self.__length)
        print(self.__width)
rect = Rectangle(5, 3)
rect.print_values()
```
## Output
<img width="1172" height="274" alt="483894205-3def9510-a203-46fb-b7a6-4a7c0e8ec6d7" src="https://github.com/user-attachments/assets/a43aaa4b-6e5b-4c8f-956a-1348d4330c4e" />

## Result
Thus, the program has been executed successfully.

## Method Overriding-Fish and Shark Class Inheritance in Python

## AIM:
To write a Python program that demonstrates class inheritance by creating a parent class Fish with a method type, and a child class Shark that overrides the type method.

## ALGORITHM:
1.Define the Fish class with a method named type() that prints "fish".
2.Define the Shark class as a subclass of Fish, and override the type() method to print "shark".
3.Create an instance of the Fish class named obj_goldfish.
4.Create an instance of the Shark class named obj_hammerhead.
5.Use a for loop to iterate over both objects.
6.Within the loop, call the type() method using the loop variable.
7.Output will demonstrate method overriding: printing "fish" and "shark" accordingly.

## PROGRAM:
```
class Fish:
    def type(self):
        print("fish")
class Shark(Fish):
    def type(self):
        print("shark")
obj_goldfish = Fish()
obj_hammerhead = Shark()
obj_goldfish.type()
obj_hammerhead.type()
```

## OUTPUT
<img width="839" height="289" alt="483894250-8ab32440-5842-4db9-838b-e29d3db8b3e6" src="https://github.com/user-attachments/assets/9641b40c-4605-4cdf-bce1-27711c959780" />


## RESULT
Thus,the program has been executed successfully.

##  Python OOP: Operator Overloading (Less Than <)

## AIM
To write a Python program that demonstrates operator overloading by overloading the less than (<) operator using a custom class.

## ALGORITHM
1.Create Class A:
   Define the init() method to initialize the object with a value a.
2.Overload the < Operator:
    Define the lt() method with logic:
    If self.a < o.a, return "ob1 is less than ob2"
    Else, return "ob2 is less than ob1"
3.Create Objects:
    Instantiate two objects ob1 and ob2 with values.
4.Use < Operator:
   Use print(ob1 < ob2) to trigger the overloaded behavior.
   
## Program
```
class A:
    def __init__(self,a):
        self.a=a
    def __gt__(self,other):
        return self.a<other.a
ob1=A(200)
ob2=A(30)
if(ob1<ob2):
    print("ob2 is less than ob1")
else:
    print("ob1 is less than ob1")
```

## Output
<img width="1177" height="268" alt="483894309-72bd2fcd-66f6-44fd-b85c-ffe7ec20336e" src="https://github.com/user-attachments/assets/4aa18c85-607d-4bea-b2d7-d6daaa15a91f" />

## Result
Thus,the program has been executed successfully.

## Python OOP: Polymorphism with Classes

## AIM
To create two specific classes — Beans and Mango. Then, create a generic function that can accept any object and determine its type (Fruit or Vegetable) and color, using polymorphism.

## ALGORITHM
1.Create Class Beans:
   Define type() method that prints "Vegetable".
   Define color() method that prints "Green".
2. Create Class Mango:
   Define type() method that prints "Fruit".
   Define color() method that prints "Yellow".
3.Define Generic Function func(obj):
    Call obj.type() and obj.color() — this works with both Beans and Mango objects, showcasing polymorphism.
4.Create Objects:
    Instantiate Beans and Mango.
    Pass them to func() and execute the program.
    
## Program
```
class Beans(): 
     def type(self): 
       print("Vegetable") 
     def color(self):
       print("Green") 
class Mango(): 
     def type(self): 
       print("Fruit") 
def color(self): 
       print("Yellow")
obj_beans = Beans() 
obj_mango = Mango()
for func in (obj_beans,obj_mango): 
    func.type()
    func.color()
```

Output
<img width="1181" height="342" alt="483894381-dee6b806-7c2f-421c-9162-d86717bc5be0" src="https://github.com/user-attachments/assets/45b332c2-412a-4f45-86d4-94cf5e609b22" />

## Result
Thus,the program has been executed successfully.

