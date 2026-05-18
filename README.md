# Product Management System Frontend

This is an Angular / TypeScript frontend project for a Product Management System. The application provides user interface workflows for product CRUD operations, user registration, login workflows, and REST API integration with a Spring Boot backend.

## Tech Stack

- Angular
- TypeScript
- JavaScript
- HTML
- CSS
- Bootstrap
- REST API Integration

## Features

- Product list page
- Add product workflow
- Edit product workflow
- Product detail view
- Delete product workflow
- User registration page
- User login page
- Dashboard routing
- Angular service-based API communication
- Integration with Spring Boot backend REST APIs

## Frontend Structure

```text
Angular Application
        ↓
Components
        ↓
Services
        ↓
Models
        ↓
HTTP Client
        ↓
Spring Boot REST API
```

## Main Components

### ListProductComponent

Displays the list of products retrieved from the backend API.

### AddProductComponent

Provides a form workflow for creating a new product.

### EditProductComponent

Provides a form workflow for updating an existing product.

### DetailProductComponent

Displays details for a selected product.

### RegistrationComponent

Provides the user registration workflow.

### LoginComponent

Provides the user login workflow.

### DashboardComponent

Provides dashboard navigation after user login.

## Services

### ProductService

Handles HTTP requests for product CRUD operations.

Backend endpoint used:

```text
http://localhost:8090/product/prd
```

### UserService

Handles HTTP requests for user registration and login workflows.

Backend endpoints used:

```text
http://localhost:8090/all/users
http://localhost:8090/all/userLogin
```

## Models

### Product

Represents product data used by the Angular frontend.

Main fields:

```text
id
productname
productdescription
price
```

### User

Represents user registration and login data.

Main fields:

```text
id
email
username
password
```

## Related Backend Repository

This frontend is designed to work with the Spring Boot backend repository:

```text
product-management-system-backend
```

The backend provides REST APIs for product CRUD operations, user registration, login workflows, and MySQL database persistence.

## API Integration

The Angular frontend connects to the backend using REST APIs such as:

```text
GET     http://localhost:8090/product/prd
POST    http://localhost:8090/product/prd
GET     http://localhost:8090/product/prd/{id}
PUT     http://localhost:8090/product/prd/{id}
DELETE  http://localhost:8090/product/prd/{id}

POST    http://localhost:8090/all/users
POST    http://localhost:8090/all/userLogin
```

## Notes

This repository contains the Angular frontend for the Product Management System. The backend is maintained separately in the Product Management System backend repository.

## Future Improvements

- Improve UI styling and layout
- Add form validation
- Add route guards
- Add authentication state management
- Add error handling for API responses
- Add environment-based API configuration
- Improve responsive design
