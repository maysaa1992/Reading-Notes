# Reading Questions

## 1-What are the key characteristics of serverless computing, and how does it differ from traditional server-based architectures?

Serverless architectures have rapidly emerged as a new technology concept over recent years. Using this architecture, you can create a variety of applications for various industries. If you have a need for computation-light, highly-flexible, stateless applications, then you can familiarize yourself with the basic concepts of serverless architectures and draw inspiration from this document.



## 2-How can one get started with Vercel, and what are the main steps involved in deploying a serverless function using Vercel?


Step 1 – Deploy.


Step 2 – Configure.


Step 3 – Assign a Domain.


Step 4 – Make Changes.


Step 5 – Collaborate.


Step 6 – Add Compute.


Step 7 – Monitor



## 3-What are APIs, and how can they be utilized in Python applications to access and manipulate data from external sources?


A REST web service is any web service that adheres to REST architecture constraints. These web services expose their data to the outside world through an API. REST APIs provide access to web service data through public web URLs.

For example, here’s one of the URLs for GitHub’s REST API:

https://api.github.com/users/<username>
This URL allows you to access information about a specific GitHub user. You access data from a REST API by sending an HTTP request to a specific URL and processing the response.

## 4-What is the Requests library in Python, and how can it be used to interact with APIs by sending HTTP requests? Can you provide an example of a basic GET request using the Requests library?

Definition and Usage. The requests module allows you to send HTTP requests using Python. The HTTP request returns a Response Object with all the response data (content, encoding, status, etc)
How do you interact with APIs in Python?
To interact with an API, specifically a web API in python we can make use of the standard requests module to make the request, because most web service APIs return a response in a format known as JSON it will be useful to know little about it. JSON is a way to store data in an organized, logical manner
While we can manually send and receive data over HTTP using the socket library, there is a much simpler way to perform this common task in Python by using the urllib library. Using urllib , you can treat a web page much like a file