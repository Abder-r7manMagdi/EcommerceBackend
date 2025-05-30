REST API for My E-Commerce Application
I developed this REST API as a backend for an e-commerce platform as part of my personal/academic project. This API handles all fundamental CRUD operations required by any e-commerce system, with user authentication and authorization implemented at every step to ensure security.

E-R Diagram for the Application


Tech Stack
Java

Spring Framework

Spring Boot

Spring Data JPA

Hibernate

MySQL

Modules
Login & Logout Module

Seller Module

Customer Module

Product Module

Cart Module

Order Module

Features
Customer and Seller authentication and validation with session tokens valid for one hour to enhance security.

Seller Features:

Administrator role with full control of the application.

Only authenticated sellers with valid session tokens can add, update, or delete products.

Sellers can access details of customers and their orders.

Customer Features:

Customer registration and login to obtain valid session tokens.

Browsing products, adding items to cart, and placing orders.

Customers can only access their own orders, cart, and profile features once logged in.

Installation and Running Instructions
Update the database configuration inside the application.properties file according to your local setup (username, password, and port).

properties
Copy
Edit
server.port=8009
spring.datasource.url=jdbc:mysql://localhost:3306/ecommercedb
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.datasource.username=root
spring.datasource.password=root
Start the server and access the API at:

bash
Copy
Edit
http://localhost:8009/
http://localhost:8009/swagger-ui/index.html#/
