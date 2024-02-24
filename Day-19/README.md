# Python-DataScience-90Days-Challenge - Day19

Day 19 of the Python Data Science 90 Days Challenge is all about Exception Handling.

#### try,except and finally blocks in Python:
In this challenge we will learn how to use `try`, `except` and `finally` blocks in Python for exception handling.

```
syntax:
try:
   # code block to monitor for errors
except [exception type]: 
   # code block to execute if error occurs
finally:  
   # code block to execute regardless of an error occurring or not

```
We can also use `else`  statement with except block which will be executed only when there is no exception occurred.


#### Raise an exception manually using raise keyword:
python provides a way to generate exceptions by raising them with the `raise` statement. 

python has a built-in `Exception` class that can be used when raising exceptions. You can also define your own custom exceptions by subclassing from this.

```
syntax:
raise Exception(argument)

# Example usage:
def divide_numbers(x, y):
    try:
        result = x / y
    except ZeroDivisionError:
        print("You can't divide by zero!")
        # We could also use 'pass', but it's generally better practice to handle this specific case explicitly.
        # We could just end here but it's good practice to raise an exception instead
        raise ValueError("Can't divide by zero.")
    return result

print(divide_numbers(5, 0))

```


