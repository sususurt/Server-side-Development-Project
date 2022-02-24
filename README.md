# Server-side Development Project
> Coursera: https://www.coursera.org/specializations/full-stack-mobile-app-development .

Build and configure a backend server using NodeJS framework with RESTful API for the front-end to access backend services。


## Installation
This project uses node, npm, MongoDB(Version: 5.0.6).
1. Start mongoDB
2. Modify the mongoDB url in config.js
3. Start running the server
```sh
npm start 
```

## Usage example

### Signup

#### Username and Password

Open link https://localhost:3443/users/signup using a browser or send a `POST` request 
through postman or other api testing software by providing `username` and `password` in json format
in the body of the request.

#### Facebook OAuth 2

Open link https://localhost:3443/index.html using a browser

### Dishes

`https://localhost:3443/dishes`

#### GET

Get all the dish information in the database.

#### POST

(Admin user) Update dish information into the database.

#### DELETE

(Admin user) Delete all the dish documents in the database.

### Comments

`https://localhost:3443/dishes/:dishId/comments`

#### GET

Get all the comments for dish with `dishId` in the database.

#### POST

(Admin user) Update dish comments for dish with `dishId`.

#### DELETE

(Admin user) Delete all comments for dish with `dishId`.

`https://localhost:3443/dishes/:dishId/comments/:commentId`

#### GET

Get the specific comment with `dishId` and `commentId`

#### POST

(user who post the comment) Update dish comment for dish with `dishId` and `commentId`.

#### DELETE

(user who post the comment) Delete the comment for dish with `dishId` and `commentId`.




