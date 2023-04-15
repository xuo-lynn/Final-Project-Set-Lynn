# Video Game Store Inventory Management System
This is an inventory management system developed for a video game store using REST and GraphQL APIs, agile techniques, and test-driven development approach. This system allows the end user to manage the inventory of video games, game consoles, and T-shirts.

### Video Presentation
[![Game store video presentation](https://images.unsplash.com/photo-1637592156141-d41fb6234e71?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1553&q=80)](https://vimeo.com/814841167)

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
We followed the Agile methodology to plan and track our project in Jira, using story points to estimate our work. We used a test-driven development approach, with JUnit for unit and integration tests. We also used mock objects where appropriate and JSR303 for input validation. Our design includes a service layer and implements ControllerAdvice to handle exceptions and return proper HTTP status codes and data.

## User Stories
This application completes the following user stories:

- Users can create, read, update, and delete game information.
- Users can search for games by studio, ESRB rating, and title.
- Users can create, read, update, and delete console information.
- Users can search for consoles by manufacturer.
- Users can create, read, update, and delete T-shirt information.
- Users can search for games by color and size.
- Users can purchase a specified quantity of products (games, consoles, T-shirts) and an invoice will be created that includes any taxes and processing fees.

## API Features

### Games
The REST API allows the end user to perform standard CRUD operations for games and search for games by studio, ESRB rating, and title. There is a separate repository for games.

The GraphQL API allows the end user to retrieve the following information:

- Get all Games
- Get a Game by ID
- Get a Game by Title
- Get a Game by ESRB rating
- Get a Game by Studio


### Consoles
The REST API allows the end user to perform standard CRUD operations for consoles and search for consoles by manufacturer. There is a separate repository for consoles.

The GraphQL API allows the end user to retrieve the following information:

- Get all Consoles
- Get a Console by ID
- Get a Console by Manufacturer

### T-shirts
The REST API allows the end user to perform standard CRUD operations for T-shirts and search for T-shirts by color and size. There is a separate repository for T-shirts.

### Invoices
The REST API allows the end user to create an invoice by supplying the following information to the endpoint:

- Name
- Street
- City
- State
- Zip
- Item type
- Item ID
- Quantity

The endpoint returns invoice data based on the provided invoice table, with all invoice calculations done in the service layer. There are separate repositories for taxes and processing fees.
