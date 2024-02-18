# Python-DataScience-90Days-Challenge - Day15

Day 15 of the Python Data Science 90 Days Challenge is all about OOPS. Object Oriented Programming in Python. Today we will be learning how to create a class.

Class Syntax:
```
class <c_name>:
    code.....
```

```
class python:
    '''This is a class for python.'''
    print("hello python")
```

#### Create Object:
An object of the class can be created using the following syntax: `obj = ClassName()`
Example:  
`my_python = python()`

#### Accessing Attributes and Methods:
Attributes are accessed by using `.` operator followed by attribute name.  

Methods are called using parentheses `( )`.

Example:  

`print(my_python.attribute)` or `my_python.method()`</s>

#### the __init__() Function:
The __init__() function is a special method in Python classes that serves as a constructor. It gets called when an object is instantiated from a class and it allows the class to initialize the attributes.
```
class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age

p1 = Person("Venkat", 37)

print(p1.name)
print(p1.age)
```
#### The __str__() Function:
The `__str__()` method allows you to define what should be printed when an object is converted into a string. By default, Python uses this method to return a string representation of an object.
```
class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age

  def __str__(self):
    return f"{self.name}({self.age})"

p1 = Person("Venkat", 37)

print(p1)
```
#### Object Methods:
Objects can also contain methods. Methods in objects are functions that belong to the object.
To define a method for an object you need to use the `def` keyword along with the function name inside the class definition. They have access to any attributes of the object through the `self` keyword.
To define a method for an object, you use the `def` keyword like normal functions but put it under the class definition instead of outside of it.
```
class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age

  def myfunc(self):
    print(f"Hello my name is {self.name}")
    print(f"{self.name} is {self.age} years old")

p1 = Person("Venkat", 36)
p1.myfunc()
```
Note: The self parameter is a reference to the current instance of the class, and is used to access variables that belong to the class.

 Output: Hello my name is Venkat
        Venkat is 36 years old


##### The Self Parameter:
The `self` parameter is a reference to the current instance of the class and it allows access to the attributes of the class.

It does not have to be named self , you can call it whatever you like, but it has to be the first parameter of any function in the class:
```
class Person:
  def __init__(lol, name, age):
    lol.name = name
    lol.age = age

  def myfunc(self):
    print(f"Hello my name is {lol.name}")
    print(f"{lol.name} is {lol.age} years old")

p1 = Person("Venkat", 36)
p1.myfunc()
```
