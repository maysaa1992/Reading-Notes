# Reading Questions:
**1-Explain the concept of variable scope in Python and describe the difference between local and global scope. Provide an example illustrating the usage of both.**

Scope of Variable
A variable's scope is basically the lifespan of that variable. It is the section of code to which a variable is alive. Depending on their scope, variables are divided into:

**Global variable's**

**Local variable's**

 

**Local Variable**
Local variables are declared inside the function blocks. In Python, local variables can be declared at any location in the code block.

Only statements that are written inside a function can access local variables. They are secure in the way that no other function or variable of that program can access them 

## Example:
```
def fun():

   a=10

 print(a)
 ```

**Global Variable**
Global variables are the types of variables that are declared outside of every function of the program. The global variable, in contrast to local variables, is accessible by all functions in a program. Global variables are not very reliable because any function in the program can alter their value.

## Example:
```
a = 10

def fun():

     global a

     print(a)
 ```
**2. How do the global and nonlocal keywords work in Python, and in what situations might you use them?**

The main difference is that Global is used to access and modify global variables from within a function, while nonlocal is used to access and modify variables from the nearest enclosing scope that is not global

## Example:
```
outside function 
def outer():
    message = 'local'

    # nested function  
    def inner():

        # declare nonlocal variable
        nonlocal message

        message = 'nonlocal'
        print("inner:", message)

    inner()
    print("outer:", message)

outer()
```


**3. In your own words, describe the purpose and importance of Big O notation in the context of algorithm analysis.**


is a tool used to describe the time complexity of algorithms. It calculates the time taken to run an algorithm as the input grows.
In other words, it calculates the worst-case time complexity of an algorith