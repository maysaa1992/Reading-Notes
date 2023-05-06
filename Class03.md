# Calss03

**-What Is a File?**

file is a contiguous set of bytes used to store data. 
This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. 



**-file systems are composed of three main parts:**

**Header:** metadata about the contents of the file (file name, size, type, and so on)


**Data:** contents of the file as written by the creator or editor


**End of file (EOF):** special character that indicates the end of the file


**-File Paths**

**Folder Path:** the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows)


**File Name:** the actual name of the file


**Extension:** the end of the file path pre-pended with a period (.) used to indicate the file type

**Opening and Closing a File in Python**

When you want to work with a file, the first thing to do is to open it. This is done by invoking the open() built-in function. open() has a single required argument that is the path to the `file. open()` has a single return

| Character      | Meaning |
| -----------| ----------- |
| 'r'	      |Open for reading (default) |
| 'w'	   |Open for writing, truncating (overwriting) the file first|
|'rb' or 'wb'| Open in binary mode (read/write using byte data) |

**There are three different categories of file objects:**

**Text files**-->`open('abc.txt')`


**Buffered binary files**-->`open('abc.txt', 'rb', buffering=0)`


**Raw binary files**-->


# Reading Questions


**1-What is the purpose of the ‘with’ statement when opening a file in Python, and how does it help manage resources while reading and writing files?**

This simplifies the code because the with statement can handle closing the file after it has been utilized.


**2-Explain the difference between the ‘read()’ and ‘readline()’ methods for file objects in Python. Provide examples of when to use each method**

**Method** -->read(size=-1):

This reads from the file based on the number of size bytes. If no argument is passed or None or -1 is passed, then the entire file is read 

**Method**-->.readline(size=-1):
    This reads at most size number of characters from the line. This continues to the end of the line and then wraps back around. If no argument is passed or None or -1 is passed, then the entire line (or rest of the line) is read
    
**Briefly describe the concept of exception handling in Python. How can the ‘try’, ‘except’, and ‘finally’ blocks be used to handle exceptions and ensure proper execution of code? Provide a simple example.**
![expcption](exption.webp)
```
try:
    linux_interaction()
except AssertionError as error:
    print(error)
else:
    try:
        with open('file.log') as file:
            read_data = file.read()
    except FileNotFoundError as fnf_error:
        print(fnf_error)
finally:
    print('Cleaning up, irrespective of any exceptions.')
```
