# Building a REST API with Spring Boot

Welcome to the [**Building a REST API with Spring Boot**](https://spring.academy/courses/building-a-rest-api-with-spring-boot) project! This repository is a hands-on practice project for enhancing Spring Boot skills, created as part of the course offered by [Spring Academy](https://spring.academy/).

---

## 📚 About the Project

This project is designed to help developers practice and refine their knowledge of building robust and scalable RESTful APIs using Spring Boot. It covers fundamental to advanced concepts, including:

- Designing and implementing RESTful endpoints
- Pagination and Sorting
- Data Persistence and JSON Serialization/Deserialization
- Exception Handling
- Testing REST APIs with JUnit

The course is free and available to anyone with a work, vocational, or educational email address, making it an excellent resource. For more details, refer to this [Spring Article](https://spring.io/blog/2024/04/10/spring-academy-pro-content-now-free-to-access).

---

## 🛠 Features Implemented

- **CashCard Management**
  - Create a new CashCard
    - Tested JSON serialization and deserialization using TDD.
    - Added a POST endpoint to the REST Controller.
    - Ensured semantic correctness using `CrudRepository.save`.
  - Retrieve details of a specific CashCard
    - Added a GET endpoint to the REST Controller.
    - Tested with Spring Boot to validate functionality.
    - Utilized the `@PathVariable` annotation to pass data dynamically.
  - Retrieve all CashCards with pagination and sorting
    - Implemented a GET endpoint for retrieving a list of CashCards.
    - Supported pagination and sorting with default behaviors.
    - Combined paging and sorting functionality seamlessly.
  - Update a CashCard
    - Implemented a PUT Controller request handler.
    - Ensured only authorized users could update their CashCards.
  - Delete a CashCard
    - Added a hard delete endpoint.
    - Followed best practices to avoid revealing information to unauthorized users.

- **Security Enhancements**
  - Configured Spring Security for authentication and authorization.
  - Tested Basic Authentication.
  - Ensured only the correct CashCard owner could access or modify their records.
  - Implemented filtering by owner in the Repository to enhance security.
  - Addressed Cross-Site Request Forgery (CSRF) concerns.
  - Leveraged Spring Security's default security practices for robust error handling.

- **Testing Suite**
  - Wrote JUnit tests for endpoint validation.
  - Tested JSON serialization and deserialization.
  - Verified interaction between components using `@DirtiesContext` annotation.

- **Data Management**
  - Configured an in-memory H2 database for development.
  - Added Spring Data to the application.
  - Created the `CashCardRepository` using `CrudRepository` for persistence.
  - Used Dependency Injection to make the repository accessible throughout the application.

- **Code Practices**
  - Refactored code following the Red, Green, Refactor development loop.

---

## Prerequisites

Ensure you have the following installed:

- Java 17 or later
- Gradle 7.5 or later
- Spring Boot 3.4.1
- IDE (e.g., IntelliJ IDEA, Eclipse)
