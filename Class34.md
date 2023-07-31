# Reading Questions

## 1-What are the key principles to follow when organizing and configuring Django settings for a project, according to the “Django Settings Best Practices” reading? 

Keep settings in environment variables.
Write default values for production configuration (excluding secret keys and tokens).
Don't hardcode sensitive settings, and don't put them in VCS.
Split settings into groups: Django, third-party, project.

## 2-How does the White Noise library contribute to the efficient serving of static files in a Django application, and what are the steps to integrate it into a project?

WhiteNoise allows your Django project to serve its own static files, making it a self-contained unit that we can deploy anywhere without depending on service providers. Although it works with any WSGI-compatible web application, it is most easily configured with a Django project

To make Django aware of you wanting to run WhitNoise, you have to specify it in the MIDDLEWARE list in settings.py file: my_tennis_club/my_tennis_club/settings.py : . . 

## 3-What is the purpose of Cross-Origin Resource Sharing (CORS) in web applications, and how can it be implemented and configured in a Django project to control access to resources? 

CORS (Cross-Origin Resource Sharing) is a web securiaty feature to control cross-origin requests.

To enable CORS in a Django project:

Install django-cors-headers: pip install django-cors-headers
Configure settings: Add 'corsheaders' to INSTALLED_APPS, and 'corsheaders.middleware.CorsMiddleware' as the first middleware in MIDDLEWARE.
Specify allowed origins: Set CORS_ALLOWED_ORIGINS to a list of allowed domains or use '*' for any origin.
Optionally, configure other settings like CORS_ALLOW_CREDENTIALS, CORS_ALLOW_METHODS, and CORS_ALLOW_HEADERS.
Exempt CSRF cookie (if using CSRF protection): Add CSRF_COOKIE_SAMESITE = None to settings.py.
Restart Django server.   

