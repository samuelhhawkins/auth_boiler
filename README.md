# auth_boiler
boiler for proj 2 


This is a boiler plate for an express app with local user authentication. It exists so I have a customized boilerplate and dont have to start from scratch on all my projects 

## What it includes 

* local Auth (email and password)
* passport and passport-local
* Sessions for saving user info and displaying flash messages 
* settings forPostGreSQL and sequelize
* Hashed Passwords 
* EJS templating and EJS layouts
* sequelize user model
* Materialize styling - nav and footer 


## Models

**User Model**

| Column | Type | Notes |
| ------ | ---- | -------| ------------------- |
|  id | Integer | Serial Primary Key |
| firstname| String | Required length > 1 |
| lastname| String | - |
| password | String | unique login |
| bio | text | - |
| admin | Boolean | Defaulted to False |
| createdAt | Date | Automaticlly added by Sequelize|
| updateddAt | Date | Automaticlly added by Sequelize|

## Routes

**Routes in Index**
| Method | Path | Purpose|
| ------ | ---- | -------| ------------------- |
| GET | '/' | Home page |
| GET | '/' | Catch-all for 404s |

## Directions For Use
| Method | Path | Purpose|
| ------ | ---- | -------| ------------------- |
| GET | '/auth/login' | Render login |
| POST | '/auth/login' | Process login data |
| GET | '/auth/signup' | Render signup form |
| POST | '/auth/signup' | process signup data |
| GET | '/auth/logout' | Remove user from signup |
