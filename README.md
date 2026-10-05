# Expense Tracker

A backend-based **Expense Tracker application** built with Java and Spring Boot. The application provides a structured way to manage users and financial transactions while demonstrating REST API development, database integration, and layered backend architecture.

## 🚀 Features

- User management
- Add and manage expense transactions
- Categorize financial transactions
- Store and retrieve transaction data
- RESTful API architecture
- Spring Data JPA integration
- H2 database support for local development
- Layered architecture using Controller, Service, Repository, and Model layers

## 🛠️ Tech Stack

- **Java**
- **Spring Boot**
- **Spring Data JPA**
- **Hibernate**
- **H2 Database**
- **Maven**
- **REST APIs**

## 📁 Project Structure

```text
ExpenseTracker/
│
├── src/
│   └── main/
│       ├── java/
│       │   └── com.example.Expense.Tracker/
│       │       ├── controller/
│       │       ├── model/
│       │       ├── repository/
│       │       ├── service/
│       │       └── ExpenseTrackerApplication.java
│       │
│       └── resources/
│           └── application.properties
│
├── pom.xml
└── README.md
```

## ⚙️ Getting Started

### Prerequisites

Make sure you have the following installed:

- Java 17 or later
- Maven
- Git

You **do not need to install MySQL** for the current configuration because the application uses an H2 database for local development.

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/ExpenseTracker.git
cd ExpenseTracker
```

### 2. Run the Application

Using Maven:

```bash
mvn spring-boot:run
```

On Windows, you can also use the Maven wrapper:

```powershell
.\mvnw.cmd spring-boot:run
```

### 3. Access the Application

Once Spring Boot starts successfully, the backend will run on:

```text
http://localhost:8080
```

## 🗄️ Database

The project currently uses **H2 Database** instead of MySQL, making local setup simple and eliminating the need for a separate database server.

The database configuration is located in:

```text
src/main/resources/application.properties
```

Current configuration uses an in-memory H2 database:
```

## 🏗️ Architecture

The application follows a layered backend architecture:

```text
Client
  │
  ▼
Controller
  │
  ▼
Service
  │
  ▼
Repository
  │
  ▼
H2 Database
```

### Controller

Handles incoming HTTP requests and exposes REST endpoints.

### Service

Contains the application's business logic and acts as the bridge between controllers and repositories.

### Repository

Uses Spring Data JPA to communicate with the database.

### Model

Contains the application's entities, including:

- `User`
- `Transaction`

## 🔮 Future Improvements

Potential improvements include:

- User authentication and authorization
- JWT-based security
- Expense and income dashboards
- Monthly and yearly spending analytics
- Transaction filtering and search
- Budget management
- Recurring expenses
- PostgreSQL/MySQL production database support
- API documentation with Swagger/OpenAPI
- Frontend application using React
- Docker support

## 📌 Learning Goals

This project demonstrates practical implementation of:

- Spring Boot application development
- REST API design
- Dependency Injection
- Spring Data JPA
- Hibernate ORM
- Database integration
- Layered architecture
- Maven dependency management
- Backend application development

## 👨‍💻 Author

**Pratham Jasuja**

⭐ If you find this project useful, consider giving the repository a star!