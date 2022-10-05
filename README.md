# Cinema project
<br/>**Project description:**
<br/> A simple web application, which has been written using Spring technologies, that supports authentication, authorization, and CRUD operations(see project's features). There are two roles in the project: users and admins. Users are able to get the information about movies, cinema halls, add tickets to their shopping carts and complete orders. Admins can create information about movies, add cinema halls, change and delete information about it.
<br/>
<br/>**Features:**
<br/>:arrow_forward: Authentication, authorization and creating of new users;
<br/>:arrow_forward: Assigning specific roles(USER, ADMIN);
<br/>:arrow_forward: Adding new movies and cinema halls;
<br/>:arrow_forward: Combining movies and cinema halls in movie sessions;
<br/>:arrow_forward: Adding movie sessions to a ticket;
<br/>:arrow_forward: Adding tickets to shopping carts of a specific user;
<br/>:arrow_forward: Completing an order by adding all needed information to it;
<br/>:arrow_forward: Role access to specific resources for ADMIN and for USER is configured using the following rules:
<br/>
- POST:   /register - all
- GET:    /cinema-halls - user/admin
- POST:   /cinema-halls - admin
- GET:    /movies - user/admin
- POST:   /movies - admin
- GET:    /movie-sessions/available - user/admin
- POST:   /movie-sessions - admin
- PUT:    /movie-sessions/{id} - admin
- DELETE: /movie-sessions/{id} - admin
- GET:    /orders - user
- POST:   /orders/complete - user
- PUT:    /shopping-carts/movie-sessions - user
- GET:    /shopping-carts/by-user - user
- GET:    /users/by-email - admin

<br/>**Database structure:**
![schema_dependencies](https://user-images.githubusercontent.com/101473233/193642813-f8e6af1d-599d-457a-b03a-b0b82817dccf.png)

<br/>**Technologies that were used in the project:**
<br/>- Java (11);
<br/>- Apache Tomcat 9.0.63;
<br/>- MySQL 8.0 CE;
<br/>- Hibernate 5.4.27;
<br/>- Spring Core;
<br/>- Spring MVC;
<br/>- Maven 3.8.0;
<br/>- Postman;
<br/>- Spring Security.
<br/>:eyes: **How to run the project:**
- You will need an installed environment Intellij Idea Ultimate 2022.1.2 to run Java code;
- You will also need installed MySQL 8.0 CE and Apache Tomcat 9.0.63;
- Clone this project using fork
- Set up DB's parameters in db.properties (driver, url, username and password from database)
- Run the Apache Tomcat.
- You can use already initialized data(from DataInitializer)
