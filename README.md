Thoughts Backend example
========================

Forked from this project: [Hands-On-Docker-for-Microservices-with-Python](https://github.com/PacktPublishing/Hands-On-Docker-for-Microservices-with-Python).

It is a [Flask](https://flask.palletsprojects.com/en/1.1.x/) application that creates a RESTful backend to store microblogging posts.


**THIS IS AN EXAMPLE WEBSITE FOR LEARNING PURPOSES**


What knowledge does it cover?
------
- Create a RESTful web service.
- Secure API by using JWT based Authorization.
- Expose API documentation with Swagger.
- Build, run and test services with Docker.
- Continuos integration and deployment with Travis CI.


Dependencies
------

ThoughtsBackend uses **Flask** as a web framework, **Flask RESTplus** for creating the interface, and **SQLAlchemy** to handle the database models. It uses a SQLlite database for local development.


Set it up
------

Create a virtual environment and install the requirements

    $ python3 -m venv ./venv
    $ source ./venv/bin/activate
    $ pip install -r requirements.txt


Get the local database ready

    $ python init_db.py

Start the development server

    $ FLASK_APP=wsgi.py flask run
    * Serving Flask app "wsgi.py"
    * Environment: production
    WARNING: Do not use the development server in a production environment.
    Use a production WSGI server instead.
    * Debug mode: off
    * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit

Check the service at http://127.0.0.1:5000/


Tests
------

Run the unit tests with

    $ pytest

