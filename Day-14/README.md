# Python-DataScience-90Days-Challenge - Day14

Day 14 of the Python Data Science 90 Days Challenge is all about Functions. In this day, we will be learning how to define and use functions in Python.

#### Function syntax
```
def function_name():
    print("something")
-----
function_name()

```
##### Example:
```
#adding of 2 numbers
def add(num1,num2):
    print(num1+num2)

-----
add(5,3)   # Output: 8
```

Arguments: These are the values that you pass to a function when you call it. In our example "5" and "3" were passed as arguments to the `add` function.

##### Parameters or Arguments? 
---------------------------
In the above example `num1` and `num2` are parameters. They are placeholders for values that will be passed into the function when it is called.
From a function's perspective:

A parameter is the variable listed inside the parentheses in the function definition.

An argument is the value that is sent to the function when it is called.

Number of Arguments: A function can have any number of arguments (even zero).

By default, a function must be called with the correct number of arguments. Meaning that if your function expects 2 arguments, you have to call the function with 2 arguments, not more, and not less.
```
def my_function(fname, lname):
  print(fname + " " + lname)

my_function("Venkat", "M")
```
##### Arbitrary Arguments, *args
If you do not know how many arguments that will be passed into your function, add a * before the parameter name in the function definition.

If you want your function to accept any number of arguments, you use *args. This special syntax allows you to pass a variable number of unnamed arguments to your function. Here’s an example
```
def my_function(*kids):
  print("The youngest child is " + kids[2])

my_function("KSM", "KTM", "NKM")

```
##### Keyword Arguments
Keyword arguments are used when you want to pass additional information to your function and don’t  necessarily care about their order. They allow you to send multiple values at once using keyword-value pairs
```
def my_function(child1,child2, child3):
  print("The youngest child is " + kids[2])

my_function(child1="KSM",child2="KTM", child3="NKM")

```
##### Arbitrary Keyword Arguments **kwargs
**kwargs allows you to pass additional parameters to your function without knowing what they will be named beforehand **kwargs allows you to pass additional parameters to your function and assign them as keyword arguments.   

```
def my_function(**kid):
  print("His last name is " + kid["lname"])

my_function(fname = "KS", lname = "M")
```

##### Default Values for Function Parameters
You can assign a default value for a parameter using the equals (=) operator. If no argument is passed for this parameter, Python will use the default value instead.
You can assign a default value for a parameter using the following syntax: paramName=defaultValue
If no argument is passed for this parameter, the default value will be used instead.

```
def my_function(country = "India"):
  print("I am from " + country)

my_function("USA")
my_function("France")
my_function()
my_function("UK")
```
##### Passing a list  as an argument to a function that expects individual arguments
In Python, you can pass a list (or any iterable object) as an argument to a function that expects individual arguments. The function receives each item in the list as a separate argument.

```
def my_function(food):
  for x in food:
    print(x)

fruits = ["apple", "banana", "cherry"]

my_function(fruits)
```

##### Return values from functions 
A function without a return statement returns None by default. If you want your function to produce something useful, you must include a return statement with an expression that produces the desired result.
```
def my_function(x):
  return 5 * x

print(my_function(3))
print(my_function(5))
print(my_function(9))
```
##### pass statement
The `pass` statement is a null operation; when it executes, nothing happens. It is useful as a placeholder when a statement is required syntactically, but no code needs to execute.
```
def myfunction():
  pass
```