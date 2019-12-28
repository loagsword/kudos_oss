# kudos_oss

A Simple CRUD App with Python, Flask, and React
The project is based on Build a Simple CRUD App with Python, Flask, and React by OktaDev
https://dev.to/oktadev/build-a-simple-crud-app-with-python-flask-and-react-30k5


**Section 1:** <br>
The backend will be able to implement the following user stories:

* As an authenticated user, I want to favorite a github open source project.
* As an authenticated user, I want to unfavorite a github open source project.
* As an authenticated user, I want to list all bookmarked github open source projects I’ve previously favorited.

A normal ReST API will expose endpoints so clients can create, update, delete, read and list all resources.     


**Section 2:**
The frontend will be able to implement the following user stories:

* An authenticated user should be able to search through the Github API, the open source projects of his/her preferences. 
* An authenticated user should be able to bookmark open source projects that pleases him/her. 
* An authenticated user should be able to see in different tabs his/her previously bookmarked open source projects and the search results.
* An un-authenticated user should have access to a login page to get into the app, and an authenticated user should be able to logout when desired.


**NOTES:** <br>
* Application uses mongoDB, Mongo is launched using docker-compose
```
docker-compose up
```


* From the root directory flask can be started using flask run. 
```
export MONGO_URL=mongodb://mongo_user:mongo_secret@0.0.0.0:27017/        
FLASK_APP=$PWD/app/http/api/endpoints.py FLASK_ENV=development pipenv run python -m flask run --port 4433
```

* Web app is started with `yarn start` from the `$app/http/web/app` directory. 
```
yarn start
```

* Finally note, Okata Domain and ClientID can be obtained by creating a free developer account. A preferred authentication service can be used instead. Get a free okta developer account here: https://developer.okta.com/signup/

