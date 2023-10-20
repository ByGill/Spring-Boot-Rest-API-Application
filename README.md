# Spring-Boot-Rest-API-Application
A simple Rest API using the Spring Boot Framework in Java using postgres database

It uses the Spring Boot Framework which follows a model-DAO-service-controller framework to create the REST API.

The model layer is made up the person class which has fields of ID and name.
The data access layer consists of the person dao and the person data access service. The person data access service is the class that implements the dao and injected in the person service. The data access layer in this context consists of a fake person data access service which utilizes in-house memory and the authentic data access service which uses a jdbc template to interact with a postgres database. These two data access services contains the HTTP method functions.
The service layer contains the person service class which has HTTP method functions just like in the data access layer.
The api layer contains the person controller class which implements the mapping of the HTTP methods.

