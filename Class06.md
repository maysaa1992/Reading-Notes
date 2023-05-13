# Reading
**When to Use the Random Module in Python?**

If you want the computer to pick a random number in a given range, pick a random element from a python list, pick a random card from a deck you can use the random module in python

**Random Functions in Python**


The Random module contains some very useful functions namely randint() function, random() function, choice() function, randrange() function and shuffle() function

**The random() Function:** The random() function in the python random module is used to generate random numbers between 0 and 1.

``` 
import random
random.random() * 100 
```

**The choice() Function**

is used to select a random element from a collection object like a list, set, tuple, etc. The function takes a collection object as its input argument and returns a random element.

```
import random
myList = [2, 109, False, 10, "Lorem", 482, "Ipsum"]
random.choice(myList)
 ```

 **The shuffle() Function**
As the name suggests, the shuffle function shuffles the elements in the list in place. The shuffle() function takes a list as an input argument. 
```
from random import shuffle
x = [[i] for i in range(10)]
shuffle(x)
Output:
# print x  gives  [[9], [2], [7], [0], [4], [5], [3], [1], [8], [6]]
```

**The randrange() Function**

The randrange() function in the python random module is used to select a random element from a given range. It takes three numbers namely start, stop, and step as input argument. 
```
random.randrange(start, stop[, step])

import random
for i in range(3):
    print random.randrange(0, 101, 5)
```

**What is Risk Analysis in Software Testing and how to perform it?**

The probability of any unwanted incident is defined as Risk. In Software Testing, risk analysis is the process of identifying the risks in applications or software that you built and prioritizing them to test. After that, the process of assigning the level of risk is done. The categorization of the risks takes place, hence, the impact of the risk is calculated.
 
# Reading Questions

**1-How can the random module be utilized in Python to generate random numbers or make selections from a list, and what are some common functions available within the module?**

The random() function in the python random module is used to generate random numbers between 0 and 1.

**2- the context of software development, what is risk analysis, and what are the key steps involved in conducting a risk analysis for a software project?**


The probability of any unwanted incident is defined as Risk. In Software Testing, risk analysis is the process of identifying the risks in applications or software that you built and prioritizing them to test. After that, the process of assigning the level of risk is done. The categorization of the risks takes place, hence, the impact of the risk is calculated.

**3-What is test coverage and why is it an important (or potentially misleading) metric in software testing?**

It quantifies how much of the features being tested are covered by the test, which can be a good indicator of risk. 

**What is Big O notation, and how is it used to describe the performance of an algorithm? Give an example of an everyday task (not software related) that demonstrates O(n) time complexity.**

“Big O notation is a mathematical notation that describes the limiting behavior of a function when the argument tends towards a particular value or infinity.