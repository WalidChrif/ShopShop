# ShopShop

**ShopShop** is an e-commerce platform built using Angular for the frontend and Spring Boot for the backend. It features two interfaces: one for customers and one for administrators. The project supports multilingual functionality and offers features such as product browsing, order management, and a customizable admin dashboard.

## Features

### Customer Interface
- Browse products by category.
- Search and filter products.
- Add products to the shopping cart and checkout.
- View order history and details.
- Multilingual support (Spanish and English).

### Admin Interface
- Manage product categories.
- Add, update, and delete products.
- View and manage customer orders.
- Customizable dashboard for managing the store.

## Technology Stack

### Frontend (Angular)
- **Angular**: For building the user interface and managing the client-side logic.
- **NgRx**: State management for handling authentication and dynamic content changes.
- **ngx-translate**: Used for multilingual support.
- **PrimeNG** and **NgBootstrap**: UI component libraries for a responsive design.
- **RxJS**: For handling asynchronous operations and reactive programming.
- **HTML**, **CSS**, **Bootstrap**: For styling and layout.

### Backend (Spring Boot)
- **Spring Boot**: For building the REST API.
- **Spring Security**: For securing the application.
- **Spring Data JPA**: For database operations.
- **MySQL**: As the relational database management system.
- **Keycloak**: For authentication and authorization.
- **REST API**: For communication between the frontend and backend.

## Installation and Setup

### Prerequisites
- Node.js (for Angular)
- Java (for Spring Boot)
- MySQL (for database)
- Keycloak (for authentication)

### Frontend (Angular) Setup

1. Navigate to the `shopshop-frontend` directory.
2. Install the dependencies:
   ```bash
   npm install
   ```
3. Start the Angular development server:
   ```bash
   ng serve
   ```

### Backend (Spring Boot) Setup

1. Navigate to the `shopshop-backend` directory.
2. Install the required dependencies (Maven or Gradle).
3. Configure the application.properties file with your MySQL and Keycloak settings.
4. Run the Spring Boot application:
   ```bash
   mvn spring-boot:run
   ```

### Database Setup

1. Create a new MySQL database:
   ```sql
   CREATE DATABASE shopshop;
   ```
2. Update the database connection details in the `application.properties` file.

### Keycloak Configuration

1. Install and run Keycloak.
2. Create a realm and configure roles for both customers and admins.
3. Create clients for frontend and backend with appropriate redirect URIs.

## Usage

1. Open the customer interface by navigating to `http://localhost:4200/`.
2. Admin interface is accessible through `http://localhost:4200/admin`.
3. Manage products, orders, and categories via the admin dashboard.
