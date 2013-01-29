# Intro to Flask: Creating Your Own Static Blog Generator
### Christopher Roach


If you're a web developer, you've no doubt heard of Django&#8212;the go–to web development framework for Python. While Django is a superb framework for developing complex web applications, it can be slightly cumbersome when developing something a bit smaller. That's where knowing a good micro-framework can come in handy, and [Flask][flask] fits that use case perfectly. Not content with being just a micro-framework for small web apps, Flask&#8212;built atop the powerful [Werkzeug][werkzeug] WSGI library&#8212;has the ability to grow with the complexity of your app, making Flask, in many cases, the only framework you'll ever need. Join [Christopher Roach][croach] as he shows you how to use the Flask micro-framework through the creation of a simple static blog generator.

## Chapter 1 Getting Started

### 1 - Introduction ()

We begin by discussing the role of micro-frameworks and why you should learn one if you already know a "full power" framework such as Django. We'll also discuss how Flask can grow with your app's complexity and may, therefore, be the only framework you need to know. Finally, this lesson will point the user to the Python Power Tools video on virtuanenv and virtualenvwrapper.

### 2 - Hello Flask ()

In this lesson, we'll install Flask and create our very first "Hello World" application.

---

## Chapter 2 ???

### 3 -

### ? - Generating a Feed

This episode demonstrates how easy it is to use the underlying Werkzeug library within a Flask app by using the [AtomFeed][atom] class to generate a Atom feed for our blog.

### ? - Refactoring with Blueprints

In this episode we'll break the "blog" portion of our code out into a Blueprint.

### ? - Deployment (website)

Use fabric to deploy to S3 and/or Github Pages.

### ? - Deployment (script)

Make our script pip installable (i.e., create the setup.py file).

### ? - Errror Handlers

Use the `error_handler` decorator to create a 404 handler. (This one might be better for the "Intermediate Flask" episode where we create a non-static web application)

### ? - Custom Jinja Template Filter

Create and register a custom `date` filter.

[flask]: http://flask.pocoo.org
[werkzeug]: http://werkzeug.pocoo.org
[croach]: http://christopherroach.com
[atom]: http://werkzeug.pocoo.org/docs/contrib/atom/
