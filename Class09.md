# Reading:
## What Are Dunder Methods?
In Python, special methods are a set of predefined methods you can use to enrich your classes. They are easy to recognize because they start and end with double underscores, for **example** ```__init__ ```or ``` __str__```
```
class LenSupport:
    def __init__(self, owner, amount=0):
    def __len__(self):
        return 42
```
## What is probability?
At the most basic level, probability seeks to answer the question, "What is the chance of an event happening?" An event is some outcome of interest.
# Reading Questions

**What is the purpose of dunder methods in Python? Provide an example of a commonly used dunder method?**

In Python, special methods are a set of predefined methods you can use to enrich your classes. They are easy to recognize because they start and end with double underscores, for example __init__ or __str__
```
class LenSupport:
    def __init__(self, owner, amount=0):
    def __len__(self):
        return 42
```

**3-Describe the Python statistics module and give an example of a function within the module that can be used to perform a common statistical operation.**

The statistics module provides functions to mathematical statistics of numeric data.
 The following popular statistical functions are defined in this module.
The mean() method calculates the arithmetic mean of the numbers in a list.
```
import statistics

print(statistics.mean([2,5,6,9]))  
```