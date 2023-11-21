# Django Crash
---
Django is a very popular Python web framework designed for rapid and full-stack web app development.

Many popular apps are built on Django such as Youtube, Spotify, Dropbox, edX, and more.

## Django Model-View-Template
---
<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/build-a-personal-movie-recommender-with-django/images/django_mvt.png">

Like other web frameworks, Django splits its application logic into the following three Model-View-Controller like components:

* `Django Model` manages data modelling and database mapping as well as business logic to process data

* `Django View` describes which data is presented, but not how it is presented. Typically,
Django View delegates and renders an HTML page, which describes how the data is presented

* `Django Template` generates dynamic HTML pages to present data

When a client sends a request, the Django server routes the request to the appropriate view based on the Django URL configuration
and acts as a traditional `Controller`

## Django Models
---
Django uses `Django Models` to represent database tables and map them to objects, such as process is called ORM.

Django Models tries to make the developer’s life easier by abstracting databases and mapping objects and methods
into tables and SQL queries automatically.

You just need to define classes as Django Models, and will be later mapped to database tables accordingly.

Then you can simply use Django Models API to perform CRUD on the database tables without writing a single line of SQL

<img src='https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/build-a-personal-movie-recommender-with-django/images/django_orm.png'>

## Django Views
---
<img src='https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/build-a-personal-movie-recommender-with-django/images/django-view.png'>

In Django, a View is essentially a Python function. Such a function takes a Web request and applies the necessary logic to generate a Web response, such as the HTML contents of a Web page, a redirect, a 404 error, an XML document, an image, or any other Web response.

Often, View interacts with Django Models to get required data in the form of QuerySet or objects
to generate a Web response.

## Django Template
---
<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/build-a-personal-movie-recommender-with-django/images/django-template.png">

Django uses a template to generate dynamic Web pages which are sent back and rendered in a user’s browser.

The Django template contains static HTML elements, as well as special Python code describing how the dynamic content of HTML pages will be generated.

## Django App Development Process
---
<img src='https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/build-a-personal-movie-recommender-with-django/images/django-app-dev.png'>

Let’s look at a typical Django development process. The order of these steps may vary.

First, we create a Django project which is a container for Django apps and settings. Then we create and add one or more Django apps to the project.

In Core Development, we create Django models to model the data and create views to determine which data need to be presented to the UI. 

We also map the request URLs to our views so Django can forward requests to corresponding views via URLs. Then we can start designing and building the UI.

OK, by now you should have enough knowledge about Django to get you started on this Project.

If you have more time, you could also learn more about Django framework from many other tutorials and courses online.