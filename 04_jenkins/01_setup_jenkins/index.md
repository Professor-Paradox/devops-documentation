## In your Windows Machine Create a Spring Project

java
advanced java
jdbc basic
jpa is a orm object relation mapping with a row in a table to a object in java
mvc architecture model(data) view(presentation) controller(requests)
spring mvc
spring jpa building on top of jpa
  - jpa repository with additional functions with interfaces

Repository Layer
  - extending the spring jpa repository interface we create a student repository
Service Layer
  - student service is used to create business logic, how to get and set and manipulate data if need to.
  
  
Model (Entity) part spring mvc
  - student.java is a entity class linking to a table called student in the database with id, column annotations linking to database properties as needed.

Controller Part of spring mvc
  - student controller java file is used to accept and process the http request for our api we are creating this uses all the other layers as needed.

Since we are only creating a backend api and creating view of ui with angular we don't actually use view concept in our spring code, ususally used with jsp pages or servlets. 

USED FOR DECOUPLING THE ARCHITECTURE

can generate queries for us following this format to create a new method
findByPropertyName

