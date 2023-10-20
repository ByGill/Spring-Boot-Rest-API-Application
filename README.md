# Spring-Boot-Rest-API-Application
A simple Rest API using the Spring Boot Framework in Java using postgres database

It uses the Spring Boot Framework which follows a model-DAO-service-controller framework to create the REST API.

The model package is made up the person class which has fields of ID and name.
The dao package consists of the person dao and the person data access service which is the class that implements the dao and which is injected in the person service. The dao package consists of a fake person data access service which utilizes in-house memory and the authentic data access service which uses a jdbc template to interact with a postgres database. These two data access services contains the HTTP method functions.
The person service contains HTTP method functions just like in the DAO.
The person controller contains the HTTP method mapping.

