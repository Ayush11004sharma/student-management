Student Management System

A web-based Student Management System developed using Java, Spring Boot, Thymeleaf, and MySQL. The application is designed to manage student information through a structured web interface with a Spring Boot backend and database integration.

Overview

The Student Management System is an Enterprise Java project that demonstrates the development of a server-side web application using the Spring Boot framework.

It uses Spring MVC for handling web requests, Spring Data JPA for database operations, Thymeleaf for rendering dynamic HTML pages, and MySQL for persistent data storage.

Technologies Used

Technology

Purpose

Java 21

Programming Language

Spring Boot

Backend Framework

Spring MVC

Web Application Architecture

Thymeleaf

Server-Side Template Engine

Spring Data JPA

Database Operations

Hibernate

ORM

MySQL

Relational Database

Maven

Dependency Management and Build Tool

HTML & CSS

User Interface

Features

Student information management.

Web-based user interface.

Database integration using MySQL.

Data persistence using Spring Data JPA.

Server-side page rendering using Thymeleaf.

Input validation using Spring Boot Validation.

Add or remove individual operations such as Add, View, Update and Delete according to the functionality implemented in your application.

Project Architecture

The application follows a layered architecture:

Controller Layer: Handles incoming HTTP requests and manages application navigation.

Service Layer: Contains business logic.

Repository Layer: Performs database operations using Spring Data JPA.

Entity Layer: Represents database entities.

View Layer: Displays dynamic web pages using Thymeleaf.

Project Structure

student-management/
│
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/example/ucs067/studentmanagement/
│   │   │       ├── controller/
│   │   │       ├── service/
│   │   │       ├── repository/
│   │   │       ├── entity/
│   │   │       └── StudentManagementApplication.java
│   │   │
│   │   └── resources/
│   │       ├── templates/
│   │       ├── static/
│   │       └── application.properties
│   │
│   └── test/
│
├── pom.xml
├── mvnw
├── mvnw.cmd
└── README.md

Adjust the package and folder names to match the actual project structure.

Prerequisites

Make sure you have installed:

Java Development Kit (JDK) 21

MySQL Server

IntelliJ IDEA or Visual Studio Code

Git

Maven (optional if using the included Maven Wrapper)

Installation and Setup

1. Clone the Repository

git clone https://github.com/Ayush11004sharma/student-management.git

2. Open the Project

Open the cloned folder in IntelliJ IDEA or VS Code.

3. Configure MySQL

Create a database in MySQL:

CREATE DATABASE student_management;

4. Configure Database Connection

Update src/main/resources/application.properties with your MySQL credentials:

spring.datasource.url=jdbc:mysql://localhost:3306/student_management
spring.datasource.username=YOUR_USERNAME
spring.datasource.password=YOUR_PASSWORD

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true

Use the database and property names configured by your actual application.

5. Run the Application

On Windows, execute:

mvnw.cmd spring-boot:run

Alternatively, run the StudentManagementApplication.java class from your IDE.

6. Access the Application

Open your browser and visit:

http://localhost:8080

Screenshots

Add screenshots of your application's interface here.

Future Improvements

Improve user interface and responsiveness.

Add advanced search and filtering.

Implement role-based access control.

Add pagination and sorting.

Deploy the application to a cloud hosting platform.

Author

Ayush Sharma

GitHub: @Ayush11004sharma

License

This project is developed for educational and learning purposes.
