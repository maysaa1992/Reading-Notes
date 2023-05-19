# Reading
## List Comprehensions in Python:

 offers a shorter syntax when you want to create a new list based on the values of an existing list

-List comprehension methods are an elegant way to create and manage lists.


-In Python, list comprehensions are a more compact way of creating lists.


-More flexible than for loops, list comprehension is usually faster than other methods.

## Create a List with range()
```
# [ expression for item in list ]
digits = [x for x in range(10)]
```
## Create a List Using Loops and List Comprehension in Python
```
# create a list using a for loop
squares = []

for x in range(10):
    # raise x to the power of 2
    squares.append(x**2)
```
## Multiplying Parts of a List:

```
# create a list with list comprehensions
multiples_of_three = [ x*3 for x in range(10) ]
```
## Show the first letter of each word using Python
```
# a list of the names of popular authors
authors = ["Ernest Hemingway","Langston Hughes","Frank Herbert","Toni Morrison",
    "Emily Dickson","Stephen King"]

# create an acronym from the first letter of the author's names
letters = [ name[0] for name in authors ]
```
# Reading Questions:

**1-What is the basic syntax of Python list comprehension, and how does it differ from using a for loop to create a list? Provide an example of a list comprehension that squares the elements in a given list of integers.**

You can use a for loop to create a list of elements in three steps: Instantiate an empty list.

## Example:
```
# create a list using a for loop
squares = []
for x in range(10):
# raise x to the power of 2
squares.append(x**2)
```
**2-What is a decorator in Python?**

a design pattern in Python that allows a user to add new functionality to an existing object without modifying its structure

**3-Explain the concept of decorators in Python. How do they work, and what are some common use cases for them? Provide an example of a simple decorator function from the reading.**

You'll use a decorator when you need to change the behaviour of a function without modifying the function itself.
```
def my_decorator_func(func):

    def wrapper_func():
        # Do something before the function.
        func()
        # Do something after the function.
    return wrapper_func
```
