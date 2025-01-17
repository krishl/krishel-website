---
layout: post
title:      "Sales Web Application"
date:       2017-12-13 9:11:31 -0400
permalink:  sales_web_application
Author: Krishel Lasam
categories: 
tags: [python]
comments: false
---


Over the past 5 days, I took on a coding challenge where I needed to create a sales web application using Django REST Framework. My Python experience only consists of college semester's worth of introductory Python, but I felt confident about learning Django thanks to the Ruby on Rails and Javascript background that I have acquired throughout my time at Flatiron School. It was also very exciting at the same time, since building out a full project is the one of the best ways for me to learn a new language/framework!

I approached this project with a familiar approach that I practiced all throughout Flatiron School ever since the first week of the program - Test Driven Development.

[Django Rest Framework](https://github.com/encode/django-rest-framework) is a toolkit for building web APIS. To start off the project, I updated Python to version 3.6.3. Once that was installed, I created a virtual environment and activated it for use. Inside the virtual environment, I installed Django and Django REST Framework using pip3.

I generated a `requirements.txt` file using `pip freeze`, which functions the same as the Gemfile in Ruby on Rails - keeping all installed requirements in one place. Next, I created the initial Django project files by using `django-admin startproject backend`.

Once the files were generated, I installed Django REST Framework using pip3 and added `rest_framework` into the `INSTALLED_APPS` section of my settings.py file.

Django has the ability to hold multiple apps in a single application. I created the initial app files using `python3 manage.py startapp api`, and also added it into the `INSTALLED_APPS` section in my settings.py.

- WRITING TESTS

The first step of test-driven development is to write tests. I tested the `Customer` model and the `Product` model for `create` (POST request), `get` (GET request), `update` (PUT/PATCH request), and `delete` (DELETE request) functionality.


- DEFINING THE MODELS

Inside `models.py`, I defined three models: `Customer`, `Product`, and `Cart`. A Customer has a first_name and a last_initial. A Product has a name and a description. Cart has a one-to-one relationship with Customers, and a many-to-many relationship with Products.

Once I had completed defining the models, I created a new migration using `python3 manage.py makemigrations` and migrated it with `python3 manage.py migrate`. 

- CREATING THE SERIALIZERS

The main purpose of serializers is to translate the data obtained from the database into a more readable formats, such as JSON. I used `ModelSerializer` to help create appropriate serializers according to what is defined in my models.

- IMPLEMENTING THE VIEWS

I used `ListCreateAPIView` and `RetrieveUpdateDestroyAPIView` from the generic views provided by Django REST Framework. ListCreateAPIView provides the GET and POST method handlers, while RetrieveUpdateDestroyAPIView provides GET, PUT, PATCH, and DELETE method handlers. They also provide useful save and deletion hooks such as `perform_create` and `perform_update`. I specified the queryset and serializer for each view.

- DEFINING THE URL ENDPOINTS

I defined the URL endpoints inside my app's `urls.py`, giving each endpoint a name so that tests are able to access it. Lastly, I added the urls.py file onto the main project's urls.py file. Here is a list of all of my endpoints:

```
/customers/
/customers/1/
/customers/1/cart
/products/
/products/1
/carts/
/carts/1
```

- CHALLENGES FACED

While working through this project, I came across difficulties with adding and removing products to a customer's cart. I thought of many ways to achieve this functionality. One way of going about this was to create an intermediary model called `CartProduct` and give it attributes of `product_id`, `cart_id`, and `quantity`. It would change the relationship between Cart and Products by acting as a `through` model. In this approach, I had difficulties retrieving cart_id and product_id. I believe it can be accessed via the URL, but the nesting made it difficult. Another approach I had to this problem was to use a dictionary to store the quantity. This method would remove the need for the intermediary model of `CartProduct`. I pictured the cart to be structured like this for this approach:

```
"cart": {
  "id": 1,
  "customer": 1,
  "products": [
    {"product" : ({
        "id": 1,
        "name": "product_name",
        "description": "product_id"
    }, quantity)
  }]
}
```

I tried writing functions to achieve this approach, but encountered errors regarding the inability to directly write over specific fields. The error messages suggested I use methods such as `.get()` and `.set()`.

- CONCLUSION AND FUTURE GOALS

Overall, this was a great learning experience. I enjoyed building out the app from scratch. This enabled me to learn more about the building blocks of Django as the project was forming. I still need to work on learning more of Django methods, since it seems like there are a lot available that help streamline development. My next goal is to learn more about user authorization and authentication in Django. While reading through Django resources, I found out that Django and Django REST framework excels in this area. I would love to add it as the one of the next features to this project.

The end result can be found [here](https://github.com/krishl/sales_api).
