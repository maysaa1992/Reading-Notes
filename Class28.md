# Reading Questions


## 1-How do Django Forms facilitate user input handling, and what are some key components of creating a form using the Django framework?              
  Django Forms simplify user input handling by providing an abstraction layer. Key components of creating a form in Django include defining form fields, validating input, rendering HTML forms, and handling form submission.

## 2-Explain the purpose of Django Templates in web development and describe how template inheritance can be utilized to improve code reusability and maintainability    
                                                                                                       Django Templates separate presentation logic from Python code in web development. They allow for creating dynamic web pages and utilize template inheritance to improve code reusability and maintainability. Base templates define common elements, while derived templates inherit from the base template and can override or add specific sections. This approach promotes modularity, extensibility, and easier updates

## Describe the function of Django Views in handling HTTP requests, and outline the differences between function-based views and class-based views. 
  Django has two types of views; function-based views (FBVs), and class-based views (CBVs)                                                                                                         

Django’s views have three requirements:

They are callable. A view can be either function or a class-based view. CBVs inherit the method as_view() which uses a dispatch() method to call the appropriate method depending on the HTTP verb (get, post, etc)
They must accept an HttpRequest object as its first positional argument
They must return an HttpResponse object or raise an exception.                                                                                                                                                 This function is very easy to implement and it’s very useful but the main disadvantage is that on a large Django project, usually a lot of similar     functions in the views .  
Function Based Views
Pros
Simple to implement
Easy to read
Explicit code flow
Straightforward usage of decorators
good for one-off or specialized functionality
Cons
Hard to extend and reuse the code
Handling of HTTP methods via conditional branching                                                                                                                                                            
Class Based Views
Class-based views provide an alternative way to implement views as Python objects instead of functions. They do not replace function-based views, but have certain differences and advantages when compared to function-based views.

Pros
Code reuseability — In CBV, a view class can be inherited by another view class and modified for a different use case.
DRY — Using CBVs help to reduce code duplication
Code extendability — CBV can be extended to include more functionalities using Mixins
Code structuring — In CBVs A class based view helps you respond to different http request with different class instance methods instead of conditional branching statements inside a single function based view.
Built-in generic class-based views
Cons
Harder to read
Implicit code flow
Use of view decorators require extra import, or method override