# Expense Tracker REST API using Spring Boot and MongoDB
This project implements a RESTful API for an expense tracker application using Spring Boot and MongoDB. It allows users to perform CRUD (Create, Read, Update, Delete) operations on expenses.

# Features
- Implement CRUD operations for managing expenses.
- Integrate MongoDB as the database backend.

# Setup Instructions
# Prerequisites
- Java Development Kit (JDK) installed
- Apache Maven installed
- MongoDB installed

# Running the Application Locally
Clone the repository:
`git clone <repository_URL>
`
Navigate to the project directory:
`cd expense-tracker-api
`
Configure MongoDB properties:
- Open src/main/resources/application.properties file.
- Update the MongoDB hostname, port, and database name.

Run the application:
`mvn spring-boot:run
`
# Endpoints
# Base URL
- The base URL for the API is http://localhost:8080/api/expense.
  
# Available Endpoints
- GET /api/expense - Get all expenses.
- GET /api/expense/{name} - Get an expense by Name.
- POST /api/expense - Create a new expense.
- PUT /api/expense/{id} - Update an existing expense.
- DELETE /api/expense/{id} - Delete an expense by ID.
  
# Sample Data
```[
    {
        "id": "66003d9b784ad82357393e06",
        "expenseName": "Netflix",
        "expenseCategory": "ENTERTAINMENT",
        "expenseAmount": 1500
    }
]
```
# Usage
# Creating a New Expense
Send a POST request to /api/expense with the following JSON payload:
```{
    "expenseName": "Groceries",
    "expenseCategory": "GROCERIES",
    "expenseAmount": 50.00
}
```

# Updating an Expense
Send a PUT request to `/api/expense/{id}` with the expense ID and updated JSON payload.

# Deleting an Expense
Send a DELETE request to `/api/expense/{id}` with the expense ID.
