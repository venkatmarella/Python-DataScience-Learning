# Python-DataScience-90Days-Challenge - Day5

### Data Types: 
#### Built-in:
Python has the following data types built-in by default, in these categories:

Text Type: str

Numeric Types:int, float, complex

Sequence Types:list, tuple, range

Mapping Type:dict

Set Types:set, frozenset

Boolean Type:bool

Binary Types:bytes, bytearray, memoryview

None Type:NoneType


### String Data Type:

Strings in python are surrounded by either single quotation marks, or double quotation marks.

'python' is the same as "python"

Basic usage: print("python")

#### String Methods:
Python strings is a sequence of Unicode characters that is enclosed in quotation marks. In this article, we will discuss the in-built function i.e. the functions provided by Python to operate on strings.
https://www.w3schools.com/python/python_strings_methods.asp
Methods for different datatypes can be accessed using dot (.) operator. For example, we can use .upper() method on string to make all characters uppercase.


## Type Conversion:
Python defines type conversion functions to directly convert one data type to another which is useful in day-to-day and competitive programming.
 1.Implicit Type Conversion - converts automatically by python
   Ex: a = 10
       print(type(a))
 2.Explicit Type Conversion - need human intervention to convert one data type to other.
   Ex: s="10010"
       c = int(s,2)
       print(c)
       