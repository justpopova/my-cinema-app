***Cinema-App***

This is a simplified version of the application for the cinema. This project is focused on the ability to make various
http requests (GET, POST, PUT, DELETE), with the help of which the admin and user can receive or add new information
about the movie, cinema hall, orders, movie sessions.

**Features**

1. User registration/authentication.
2. User can have user or admin role.
3. Login/logout.
4. Admin features:
- adding new movies, cinema-halls, movie-sessions
- update/remove information about movie-sessions
- get all cinema halls, movies, available movie-sessions
- find user by email
5. User features:
- complete the order
- add tickets to the shopping cart
- get all movies, cinema halls, available movie-sessions

**The project has N-Tier Architecture:**

- DAO(data access object) - all work with database at DAO layer(CRUD)
- Service - all business logic based at service layer
- Controllers - accept requests from the clients and send responses

**Technologies**

- Java 11
- Spring MVC
- Spring Security
- Hibernate
- Tomcat (9.0.50)
- Maven

**Instruction to run the project**

- Fork this repository.
- Open IntelliJ IDEA and write ```git clone <SSH link>``` in console
- Configure db.properties - set necessary parameters:

````
db.driver=YOUR_DRIVER
db.url=YOUR_URL
db.user=YOUR_USERNAME
db.password=YOUR_PASSWORD
````

For Example:

````
db.driver=com.mysql.cj.jdbc.Driver
db.url=jdbc:mysql://localhost:3306/cinema?serverTimeZone=UTC
db.user=root
db.password=1234
````

- Install Tomcat (https://tomcat.apache.org/download-90.cgi).
- Configure Tomcat Server in your IDEA.
- Run the project.
