# Intro to Flask: Creating Your Own Static Blog Generator
### Christopher Roach


If you're a web developer, you've no doubt heard of Django&#8212;the go–to web development framework for Python. While Django is a superb framework for developing complex web applications, it can be slightly cumbersome when developing something a bit smaller. That's where knowing a good micro-framework can come in handy, and [Flask][flask] fits that use case perfectly. Not content with being just a micro-framework for small web apps, Flask&#8212;built atop the powerful [Werkzeug][werkzeug] WSGI library&#8212;has the ability to grow with the complexity of your app, making Flask, in many cases, the only framework you'll ever need. Join [Christopher Roach][croach] as he shows you how to use the Flask micro-framework through the creation of a simple static blog generator.

## Chapter 1 Getting Started

### 1 - Introduction ()

We begin by discussing the role of micro-frameworks and why you should learn one if you already know a "full power" framework such as Django. We'll also discuss how Flask can grow with your app's complexity and may, therefore, be the only framework you need to know. Finally, this lesson will point the user to the Python Power Tools video on virtuanenv and virtualenvwrapper.

### 2 - Hello Flask ()

In this lesson, we'll install Flask and create our very first "Hello World" application.

Talk about what the creation of the app object does; things like:
  - sets up path information (root, templates, static, etc.)
  - sets the config
      - Two ways to do this:
          1) Through a config file - app.config.from_pyfile('settings.cfg')
              - You can also use app.config.from_envar('SETTINGS_FILE')
                to point to a file containing your config settings
          2) Through a python module - app.config.from_object(__name__)
      - In either case, only upper case attributes are added to the config

Talk about the option for running the app:
  - host: set to '0.0.0.0' to make it available externally, default to '127.0.0.1'
  - port: defaults to 5000
  - debug: Set to true to auto restart after a change

---

## Chapter 2 ???

### 3 - Templates

In this episode we create our first template and discuss template inheritance.

- Create the templates directory
  - Discuss the `template_folder` keyword argument to the Flask constructor
- Create the `base.html` template
- Create the `post.html` template

### 4 - Add the Post Class

In this episode we add a simple Post class to abstract away the details of the underlying text file.

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

### ? - Werkzeug Debugger

This episode will take a look at the powerful Werkzeug debugger that comes with Flask.

### ? - Generating URLs

This episode will cover writing URL generators for Frozen.

[flask]: http://flask.pocoo.org
[werkzeug]: http://werkzeug.pocoo.org
[croach]: http://christopherroach.com
[atom]: http://werkzeug.pocoo.org/docs/contrib/atom/
