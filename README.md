# Library_Group_Project_CICD

This project is a distributed **Library Management System** built using microservices architecture with Java and Spring Boot. The system consists of three core microservices:

- **User MicroService**: Handles user registration, login, and role management (admin or regular user).
- **Book ServiceApi**: Manages book inventory, including adding, updating, and deleting books.
- **Loan ServiceAPI**: Allows users to loan books, track loan durations, and request extensions.

Each microservice operates independently and communicates via REST APIs.

## Microservices Overview

### 1. **User MicroService**
   - **Description**: This microservice manages user-related operations like registration, login, and user role verification (admin vs regular user).
   - **Repository**: [User MicroService](https://github.com/G00408184/UserMicroService.git)

### 2. **Book ServiceApi**
   - **Description**: This microservice manages book-related operations, such as adding, updating, and deleting books from the library.
   - **Repository**: [Book ServiceApi](https://github.com/G00408184/BookServiceAPI)

### 3. **Loan ServiceAPI**
   - **Description**: This microservice handles the loaning of books, tracking of loan durations, overdue book notifications, and extensions for loans.
   - **Repository**: [Loan ServiceAPI](https://github.com/G00408184/LoanManagerAPI)

## Technologies Used
- **Java**: Core language for building the microservices.
- **Spring Boot**: Framework used for creating standalone Spring applications.
- **Docker**: Each microservice is containerized using Docker to ensure consistent deployments.
- **MySQL/PostgreSQL**: Databases used to store user, book, and loan data.
- **RabbitMQ**: For asynchronous communication between microservices (e.g., for sending overdue notifications).
- **JUnit & Mockito**: For unit testing and mocking dependencies.
- **Kubernetes**: Used to deploy and orchestrate the microservices in a cluster environment.
- **GitHub Actions**: CI/CD pipeline for automated builds, testing, and deployments.

## How to Run the Project

1. Clone each of the microservices repositories and follow the instructions in their individual `README.md` files:
   - [User MicroService](https://github.com/G00408184/UserMicroService.git)
   - [Book ServiceApi](https://github.com/G00408184/BookServiceAPI)
   - [Loan ServiceAPI](https://github.com/G00408184/LoanManagerAPI)

2. Ensure you have Docker and Docker Compose installed on your machine.

3. To run the entire application with Docker Compose, use the following command in the root directory where the `docker-compose.yml` file is located:
   ```bash
   docker-compose up --build
