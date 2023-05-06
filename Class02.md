# Reading Questions


**1-What are the key principles of Test-Driven Development (TDD) in Python, and how do they contribute to the overall quality of code?**                                                     

Test Driven Development (TDD) is software development approach in which test cases are developed to specify and validate what the code will do. In simple terms, test cases for each functionality are created and tested first and if the test fails then the new code is written in order to pass the test and making code simple and bug-free.

 **2-Explain the purpose of the if __name__ == '__main__': statement in Python scripts. What are some use cases for including this conditional in your code?** 


Execute Code When the File Runs as a Script, but Not When It's Imported as a Module. For most practical purposes, you can think of the conditional block that you open with if __name__ == "__main__" as a way to store code that should only run when your file is executed


**3-Describe the concept of recursion in Python.**

recursive function is a function defined in terms of itself via self-referential expressions.

This means that the function will continue to call itself and repeat its behaviour until some condition is met to return a result. All recursive functions share a common structure made up of two parts: base case and recursive case.     


**3-What is the difference between Python modules and packages? Explain how to create, import, and use them in your Python programs?**

 - Python Module can be a simple python File (. py extension file), i.e., a combination of numerous Functions and Global variables. A Python Package is a collection of different Python modules with an __init__.py File.   

**-To create a module:**
1. just save the code you want in a file with the file extension .py 
2. Import the module named mymodule, and call the greeting function
3. Save this code in the file mymodule.py  

4.Import the module named mymodule, and access the person1 dictionary                                                                                 

**-To create a packages**
1. Create a directory and include a __init__.py file in it to tell Python that the current directory is a package
2. Include other sub-packages or files you want                                                                                                                                                                                                 

3. Next, access them with the valid import statements.                                                                                                                                                                                              