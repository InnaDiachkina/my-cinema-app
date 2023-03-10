# Cinema Service
Cinema-Service is the functional model for business. User can display your orders and shopping cart, create new order and update shopping cart. Admin can display user by his email, add new cinema hall, movie and session movie, update data. Solid principles have been implemented in this project - code is easy to scale and maintain.

## Project structure
#### N-tier architecture with Spring

+ @Controller: the presentation tier 
+ @Service: the application logic tier 
+ @Repository: the data tier 

## Roles	Endpoints
#### Admin	
+ POST: /register
+ GET: /cinema-halls
+ POST: /cinema-halls
+ GET: /movies
+ POST: /movies
+ GET: /movie-sessions/available
+ POST: /movie-sessions
+ PUT: /movie-sessions/{id}
+ DELETE: /movie-sessions/{id}
+ GET: /users/by-email
#### User
+ POST: /register
+ GET: /cinema-halls
+ GET: /movies
+ GET: /movie-sessions/available
+ GET: /orders
+ POST: /orders/complete
+ PUT: /shopping-carts/movie-sessions
+ GET: /shopping-carts/by-user

## Used technologies
+ Apache Maven 4.0.0
+ JDK 17
+ MySQL 8.0.22
+ Tomcat 9.0.71
+ Hibernate 5.6.14
+ Spring 5.3.20
+ Spring Security 5.6.10

## You can use this project
+ fork this project
+ change parameters in db.properties
+ configure Tomcat
+ just run this
