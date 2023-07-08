# Reading Questions

## What are the key components of the Django framework, and how do they contribute to building a web application? 

                                                             Model: which is the data layer, it is the database that contains the data that the user will interact with.


View: which is the logic layer, it is the layer that contains the logic of the application, and it is the layer that connects the model and the template.


Template: which is the presentation layer, it is the layer that contains the HTML files that will be rendered to the user.


## Explain the role of Django’s MTV (Model-View-Template) architecture and how it handles a typical web request-response cycle. 


Django's MTV architecture separates concerns into models, views, and templates, enabling code organization, reusability, and maintainability throughout web development.

Request response cycle:

User sends a request to a specific URL.
Django's URL dispatcher maps the URL to the appropriate view.
The view function or class receives the request and processes data.
It interacts with models to retrieve or update data if needed.
The view selects the template for rendering the response.
The template generates HTML by incorporating dynamic data.
The rendered HTML is sent back as a response to the user's browser.
The browser receives the response and displays the rendered HTML page.

## What is the purpose of Tailwind CSS, and how does it differ from Bootstrap CSS?  

                                                                                                                        we have discussed about the two most popular framework used for front end development. Bootstrap is used for creating responsive web and mobile applications whereas Tailwind CSS is used to create customized user interfaces