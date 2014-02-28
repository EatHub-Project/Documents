#Django

![Django](./img/django.jpg)

## Philosophy
Django is a high-level Python Web framework that encourages rapid development and clean, pragmatic design. It tries to encourage the DRY Principle (Don't Repeat Yourself) with a Model-View-Template pattern.

- The **Model** manages the Data in the Database with a powerful API.

- The **View** handles HTTP requests, process them and serves a propper response. Views are mapped to urls through Regular Expressions.

- The **Template** descibes how the information is displayed to the user. It is based on Html with special tags, "{{ }}" for variables, "{% %}" for logic, to display the data provided by the view, and supports advanced features like template inheritance, Unix piping (the "|" character), and more.

## Modularity
Django is extensible through packages called "apps" that provide functionality to a project without having to implement everything from the bottom, following the DRY principle. Apps are provided by the framework or third parties. A few examples are: Administrator backend interface, user authentication and session management, REST frameworks, etc.

## Django non-rel
Django model is based on relational models. For that reason, and because we are using a NoSQL database, we are using **[Django non-rel](http://django-nonrel.org/)**, a "fork" or modification of Django which adds support for _MongoDB_ and _Google App Engine_.

## Resources
######Read them! Use them!
- [Django official documentation](https://docs.djangoproject.com/en/1.5/)
- [Django overview, basic idea](https://docs.djangoproject.com/en/1.5/intro/overview/)
- [Django starter tutorial, 5 parts](https://docs.djangoproject.com/en/1.5/intro/tutorial01/)
- [Django mongodb engine documentation](http://django-mongodb-engine.readthedocs.org/en/latest/)