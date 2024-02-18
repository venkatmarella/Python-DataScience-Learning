# Python-DataScience-90Days-Challenge - Day12

Day 12 of the Python Data Science 90 Days Challenge is all about For loops.  We will be learning how to use for loop in python and also understanding its syntax.

For loop in python  is used to iterate over a sequence (such as list, tuple or string) and execute the block of code for each iteration. 


#### For loop Syntax: 
```
for i in somthing:
    print("action")
```
#### Example: Table 
```
table_num = int(input("Enter your table number:"))
for i in range(1,11):
    print(table_num,"x",i,"=",table_num*i)
```