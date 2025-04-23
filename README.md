# Spring_E_commerce_website
This project is a fully functional e-commerce website built using Spring MVC with Hibernate for database interaction and MySQL as the underlying database. In this new version, the entire codebase has been redesigned for better reusability and modularity. Service classes now provide reusable business logic across the project, while DAO classes directly interact with the database. Hibernate configuration has been added, allowing automatic creation of databases and tables when the project runs. Several bugs have also been fixed, including issues with product images and security, and the project now supports both IntelliJ IDEA and Eclipse.

To get started, first clone the repository and open the project in your IDE. IntelliJ IDEA is recommended, but Eclipse also works. If using IntelliJ IDEA, ensure the project is opened as a Maven project and recognized as a Spring Boot application. You must also update the working directory setting in your run configuration to $MODULE_WORKING_DIR$ to allow Spring Boot to properly locate the views stored in src/main/webapp/views.

Next, configure your database connection in the application.properties file found at src/main/resources/application.properties. Use the format:

db.url=jdbc:mysql://[ip address]:[port]/ecommjava?createDatabaseIfNotExist=true  

db.username=[your username]  

db.password=[your password]  

Login Credentials: 
If you’ve executed the basedata.sql script, the following users are available:

Admin: admin / 123

User: lisa / 765

Application Structure:
Controllers handle endpoint mappings and pass data to views using ModelAndView. For example, accessing /login renders adminlogin.jsp from the views directory. Models define the data entities and relationships, while views (JSP files) are responsible for rendering content using the data provided by controllers.


Common Endpoints:
/

/register

/admin/products

/admin/customers

/admin/categories

/admin/Dashboard
