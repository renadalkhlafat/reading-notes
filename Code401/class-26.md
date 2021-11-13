# What is Django?
It is free and open source python-based web framework that enables rapid development of secure and maintainable websites ,also it help us write software that is complete ,versatile , secure ,scalable ,maintainable and portal.

## How Django Works Behind the Scenes
Django’s code is open source and available to all. Django’s organization is managed by a non-profit, the DSF, with a miniscule budget. And Django code is lead by a core team of volunteers, two paid Django Fellows, and a larger group of contributors.

### What does Django code look like?
![django](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Introduction/basic-django.png)

+ **URLs**: While it is possible to process requests from every single URL via a single function, it is much more maintainable to write a separate view function to handle each resource

+ **Templates**: A template is a text file defining the structure or layout of a file (such as an HTML page), with placeholders used to represent actual content

+ **View**: A view is a request handler function, which receives HTTP requests and returns HTTP responses. Views access the data needed to satisfy requests via models, and delegate the formatting of the response to templates.

+ **Models**: Models are Python objects that define the structure of an application's data, and provide mechanisms to manage (add, modify, delete) and query records in the database.