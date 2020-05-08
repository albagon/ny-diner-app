# New York Diner App

## Introduction

In this project, my goal is to apply all the new skills I've learned at
Udacity's Full-Stack Developer Nanodegree. Some of these skills are:

* Coding in Python 3
* Relational Database Architecture
* Modelling Data Objects with SQLAlchemy
* Internet Protocols and Communication
* Developing a Flask API
* Authentication and Access
* Authentication with Auth0
* Authentication in Flask
* Testing Flask Applications
* Deploying Applications


The **New York Diner App** application will be deployed, managed and scaled in
[Heroku](https://www.heroku.com/platform), a popular cloud platform. Another
tool used in this project is [Gunicorn](https://gunicorn.org/), a pure-Python
HTTP server for WSGI applications.

## General Specifications

1. Models will include at least…
* Two classes with primary keys at at least two attributes each
* One-to-many relationship between classes

2. Endpoints will include at least…
* Two GET requests
* One POST request
* One PATCH request
* One DELETE request

3. Tests will include at least….
* One test for success behaviour of each endpoint
* One test for error behaviour of each endpoint


## About the Stack

I have started this application based on a previous project I finished for my
Front-End Developer Nanodegree at Udacity. The original repository can be found
[here](https://github.com/albagon/restaurant-reviews).

### Backend

This application features a complete Flask-SQLAlchemy server with a set of
endpoints. Auth0 has been integrated for authentication.

The original website sources its data from a JSON file but now, a new Postgresql
Database has been integrated, along with other authentication features.

Two models are created in the database:
1. Restaurants
2. Reviews

### Auth0 Specifications

1. Create a new Auth0 Account
2. Select a unique tenant domain
3. Create a new Regular Web Application
4. Create a new API
5. Create the `.env` file in the root of your app and add your Auth0 variables and values to it.
```
# .env
AUTH0_CLIENT_ID=YOUR_AUTH0_CLIENT_ID
AUTH0_DOMAIN=YOUR_AUTH0_DOMAIN
AUTH0_CLIENT_SECRET=YOUR_CLIENT_SECRET
AUTH0_AUDIENCE=YOUR_AUDIENCE
AUTH0_CALLBACK_URL=YOUR_CALLBACK_URL
```

### Running the server

Remember to “cd” into the application’s folder. To run the development server:

1. Initialize and activate a virtual environment 
```
$ python3 -m venv env
$  source env/bin/activate
```
2. Install the dependencies:
```
$ pip3 install -r requirements.txt
```
3. Set the environment variables:
```
$ export DATABASE_URL=the_url_to_your_local_database
$ export FLASK_APP=app.py
$ export FLASK_DEBUG=True
$ export FLASK_ENV=development
```
4. Create all the tables and run the server
```
$ flask db upgrade
$ flask run
```
5. Navigate to Home page [http://localhost:5000](http://localhost:5000)

### DEPLOYED AT HEROKU
Visit [New York Diner App live](https://nydinerapp.herokuapp.com/).

## Frontend

Templates for login and logout have been added to this project.

### Leaflet.js and Mapbox:

This repository uses [leafletjs](https://leafletjs.com/) with [Mapbox](https://www.mapbox.com/).
Mapbox is free to use, and does not require any payment information.

### Note about ES6

Most of the code in this project has been written to the ES6 JavaScript specification for compatibility with modern web browsers and future proofing JavaScript code. As much as possible, this repository will try to maintain use of ES6 in any additional JavaScript added to it.

## Contributing

This repository is the result of a project I am working on to finish a Full-Stack Developer Nanodegree Program. Therefore, all contributions are welcome.

## License

New York Diner App is distributed under the [MIT license](LICENSE).
