# Python-DataScience-90Days-Challenge - Day18

Day 18 of the Python Data Science 90 Days Challenge is all about file handling. In this day, we will be learning how to read and write files in Python using different methods:

The key function for working with files in Python is the open() function. The open() function takes two parameters; filename, and mode.

"r" - Read - Default value. Opens a file for reading, error if the file does not exist

"a" - Append - Opens a file for appending, creates the file if it does not exist

"w" - Write - Opens a file for writing, creates the file if it does not exist

"x" - Create - Creates the specified file, returns an error if the file exists

"t" or "b" - Text vs Binary - Default is text mode ("t") 

`syntax:
    file = open(filename [, mode])`

Note: Make sure the file exists, or else you will get an error.


 read:
 python_file = open("python_challenge.txt", 'r')
 data = python_file.read()
 print(data)    

 append:
 python_file = open("python_challenge.txt", 'a')
 lines_to_add = "\nThis line was added using the append function."
 python_file.write(lines_to_add)

 write:
 new_file = open("new_file.txt", 'w')
 content = "This is some content that I want to add to the new file.\nAnd this is another line of content."
 new_file.write(content)
 new_file.close()

 create:
 try:
     x_file = open("file_that_does_not_exist.txt", 'x')
 except FileExistsError:
     print("The file already exists.") 
