# Reading Questions

## 1-What is the primary purpose of JSON Web Tokens (JWTs) and how do they work in terms of encoding and decoding data? 
                                                                JWTs are a good way of securely transmitting information between parties because they can be signed, which means you can be certain that the senders are who they say they are. Additionally, the structure of a JWT allows you to verify that the content hasn't been tampered with  

First, remember that JWTs are tokens that are often used as the credentials for SSO applications (mostly for OAuth 2.0). ...
Fill out the header. ...
Fill out the payload. ...
Fill out the signature with either an RSA Private Key for RS56 or HS256 passcode. ...
Press the Encode button.
Enjoy your newly created JWT.

## 2-How does JWT Authentication integrate with Django REST Framework to secure API endpoints, and what are the key components involved in this process?

JWT is an encoded JSON string that is passed in headers to authenticate requests. It is usually obtained by hashing JSON data with a secret key. This means that the server doesn't need to query the database every time to retrieve the user associated with a given token


## 3-Why is Django’s built-in runserver not suitable for production environments, and what are some alternative server options that should be considered for deploying a Django application? 

runserver lacks production readiness due to its single-threaded nature and security concerns. Alternative server options include Gunicorn, uWSGI, nginx, and Apache, which offer better performance, scalability, and security. Docker and Kubernetes help with containerization and orchestration, while cloud platforms like AWS, Google Cloud, and Azure provide services for deploying Django applications.