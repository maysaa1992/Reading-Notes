# Reading Questions
## 1-What are the key components and purpose of Django Rest Framework (DRF) permissions, and how do they help in securing an API?                               Django Rest Framework (DRF) permissions are key components that control access to API resources. 
They help secure the API by defining who can perform specific actions (e.g., read, write) on certain endpoints based on user roles or authentication status.

## 2-In SQL, what is the purpose of the SELECT statement, and how would you use it to retrieve all columns from a table called ‘employees’? 

                             query or SELECT statement is a command which gives instructions to a database to produce certain information(s) from the table in its memory. The SELECT command starts with the keyword SELECT followed by a space and a list of comma separated columns. A * character can be used 

SELECT *
    FROM employees;

## 3-Can you explain the role of DRF Generic Views and provide examples of their usage in building a RESTful API?

DRF Generic Views are a set of already implemented views that can be used to perform common tasks. They are used to simplify the creation of RESTful APIs.

from rest_framework.permissions import IsAuthenticated
from rest_framework.response import Response
from rest_framework.views import APIView

class ExampleView(APIView):
    permission_classes = [IsAuthenticated]

    def get(self, request, format=None):
        content = {
            'status': 'request was permitted'
        }
        return Response(content)

        ```

https://github.com/Mohammad-Shiyyab/Reading-Notes-401/blob/main/all.md/class-32.md