# Store Inventory Management System
This is an inventory management system developed for a video game store using REST and GraphQL APIs, agile techniques, and test-driven development approach. This system allows the end user to manage the inventory of video games, game consoles, and T-shirts.

## Back-End Structure
The solution is built using Spring Boot and Spring MVC, with JPA to interact with the back-end MySQL database. The back-end API includes controllers, services, repository, Java data objects, and unit tests.

## Technology Stack
The project was built with the following technologies:

- Spring Boot 2.7.7
- Spring MVC
- Spring Web
- JDBC API
- MySQL Driver
- Spring for GraphQL
- JPA (Java Persistence API)
- JUnit
- Mockito
- JSR303


## Methodology
Agile methodology to plan and track project in Jira, using story points to estimate work. Used a test-driven development approach, with JUnit for unit and integration tests. Also used mock objects where appropriate and JSR303 for input validation. Design includes a service layer and implements ControllerAdvice to handle exceptions and return proper HTTP status codes and data.



The endpoint returns invoice data based on the provided invoice table, with all invoice calculations done in the service layer. There are separate repositories for taxes and processing fees.
