```
Write a function called “line” that accepts a string as an argument. Your function should generate a string pattern based on the argument provided. Here are the rules:
(1) if the string provided is a number, and that number is even, generate a pattern of hash signs. For example, calling line(“4”) will generate the following:
####
and calling line(“10”) will generate the following: ##########
(2) if the string provided is a number, and that number is odd, generate a pattern of stars. For example, calling line(“3”) will generate the following:
***
and calling line(“9”) will generate the following:
*********
(3) if the string provided is not a number you can simply generate an empty
string.
Once you have generated your pattern you should return the result when completed. You cannot assume anything about the supplied string, and your function should avoid raising any exceptions that will cause your program to crash. If an exception is raised you can return an empty string.
```
---
```
Given the data file below (datafile.txt), what will be stored in the file at the end of this program?
datafile.txt
snow
snowflake
sled
sledding


file_object = open("datafile.txt", "r")
data = file_object.read()
file_object.close()
x = data.split("\n")
file_object_2 = open("datafile.txt", "w")
for i in x:
    if len(i) % 2 == 0:
        file_object_2.write(i + "!\n")
    else:
        file_object_2.write(i + "?\n")
file_object_2.close()
```
