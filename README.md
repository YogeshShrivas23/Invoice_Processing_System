# Invoice Processing System

The **Invoice Processing System** is a web-based application designed to streamline the management of invoices efficiently. It provides features like invoice creation, approval workflows, payment tracking, and reporting. The project is built using **Java Spring Boot** for the backend and **React.js** for the frontend, with **PostgreSQL** as the database.

## Table of Contents
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Environment Variables](#environment-variables)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Key Components](#key-components)
  - [Invoice Management](#invoice-management)
  - [User Authentication](#user-authentication)
  - [Role-Based Access Control](#role-based-access-control)
  - [Payment Tracking](#payment-tracking)
- [License](#license)

## Features
- **Invoice Creation:** Users can generate invoices with itemized details.
- **Approval Workflow:** Multi-level approval process for invoice validation.
- **Payment Tracking:** Track payment status of invoices.
- **User Authentication:** Secure login with role-based access.
- **Reporting & Analytics:** View reports on invoices and payments.
- **Database Integration:** Stores invoice records securely in **PostgreSQL**.

## Technologies Used
- **Backend:** Java, Spring Boot, Hibernate
- **Frontend:** React.js, Redux, Bootstrap
- **Database:** PostgreSQL
- **Authentication:** JWT-based authentication with Spring Security
- **API Documentation:** Swagger UI

## Installation
### Clone the Repository:
```sh
 git clone https://github.com/YogeshShrivas23/Invoice-Processing-System.git
 cd Invoice-Processing-System
```

### Backend Setup:
```sh
 cd server
 mvn clean install
 mvn spring-boot:run
```

### Frontend Setup:
```sh
 cd client
 npm install
 npm start
```

### Database Setup:
1. Install PostgreSQL and create a database named `invoice_db`.
2. Update the `.env` file with your database credentials.

## Environment Variables
Create a `.env` file in the root directory and configure the following:
```env
DB_USER=your_db_user
DB_HOST=your_db_host
DB_NAME=invoice_db
DB_PASSWORD=your_db_password
DB_PORT=5432
JWT_SECRET=your_jwt_secret
```

## Usage
- **Home Page:** The root route (`/`) renders the homepage.
- **Login Page:** `/login` allows users to authenticate.
- **Invoice Dashboard:** `/dashboard` displays all invoices.
- **Create Invoice:** `/create-invoice` allows new invoice creation.
- **Approve Invoice:** `/approve/:id` enables admin approval.

## Project Structure
```
Invoice-Processing-System/
├── client/            # React Frontend
├── server/            # Spring Boot Backend
├── database/          # PostgreSQL Scripts
├── .env               # Environment Variables
├── README.md          # Project Documentation
└── package.json       # Frontend Dependencies
```

## Key Components
### Invoice Management
- Create, update, delete invoices.
- Assign invoices to specific users.

### User Authentication
- Uses JWT-based authentication for security.
- Login and registration features.

### Role-Based Access Control
- Admins can approve or reject invoices.
- Users can create and track invoices.

### Payment Tracking
- Track invoice payments with status updates.
- Generate reports on pending and completed payments.

## License
This project is licensed under the MIT License. See the `LICENSE` file for more details.

--- 

