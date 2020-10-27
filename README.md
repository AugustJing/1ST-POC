eCommerce:
It's a shopping website for HitltonToHome.

E-Commerce Microservices Backend POC using Spring Cloud

Eureka Discovery Server : 
Holds the information about all the client microservices i.e Admin and User microservice. All clients register themselves with eureka server and use it to communicate with each other.

Config Server : 
Centralized configuration server which facilitates external configuration. Client Microservices connect to this server to obtain necessary configuration information(eg: database host and port). The configuration file can be backed by a version control system like git.

Admin Microservice : 
Serves all the endpoints related to product catalog. Enables administrator of the website to add/update/delete products. MongoDB is used to store product related details.

User Microservice : 
Serves all endpoints related to user such as login by email, new user enrolment, editing existing user profile, fetching user profile details. PostgreSQL is used to store user details. Hibernate ORM is used to interact with PostgreSQL.
