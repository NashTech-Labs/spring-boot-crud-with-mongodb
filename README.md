# Spring Boot MongoDB CRUD example - Restful CRUD API

Overview of Spring Boot MongoDB CRUD example
We will build a Spring Boot MongoDB Rest CRUD API for a Tutorial application in that:

Each Tutotial has id, title, description, published status.
Apis help to create, retrieve, update, delete Tutorials.
Apis also support custom finder methods such as find by published status or by title.

#### Technology

Java 8
Spring Boot 2.6.3 (with Spring Web MVC, Spring Data MongoDB)
MongoDB
Maven 3.6.1

#### Create & Setup Spring Boot project
Use Spring web tool or your development tool (Spring Tool Suite, Eclipse, Intellij) to create a Spring Boot project.

Then open pom.xml and add these dependencies:

<dependency>
	<groupId>org.springframework.boot</groupId>
	<artifactId>spring-boot-starter-web</artifactId>
</dependency>
<dependency>
	<groupId>org.springframework.boot</groupId>
	<artifactId>spring-boot-starter-data-mongodb</artifactId>
</dependency>

#### Configure Spring Data MongoDB
Under src/main/resources folder, open application.properties and add following lines.

spring.data.mongodb.database=knoldus_tutorial_db
spring.data.mongodb.port=27017
Define Data Model
Our Data model is Tutorial with four fields: id, title, description, published.
In model package, we define Tutorial class.

## Run Spring Boot application
```
mvn spring-boot:run
```
# spring-boot-crud-with-mongodb
