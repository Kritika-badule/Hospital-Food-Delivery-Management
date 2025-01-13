# Hospital Management System

## Overview

The **Hospital Management System** is a comprehensive web application designed to manage patient meals efficiently. It facilitates three user roles: **Manager**, **Inner Pantry Staff**, and **Delivery Personnel**, each with specific functionalities tailored to their responsibilities.

## Features

### Manager Dashboard
- **Create Diet Charts**: Define meals for patients with meal time, ingredients, and instructions.
- **Manage Inner Pantry**: Add pantry staff, assign food preparation tasks.
- **Track Meal Status**: Monitor preparation and delivery statuses via a dynamic table.

### Inner Pantry Staff Dashboard
- **Manage Food Preparation**: Update meal preparation statuses (e.g., In Progress, Completed).
- **Manage Delivery Personnel**: Add delivery personnel and assign tasks.
- **Track Deliveries**: View and manage delivery details.

### Delivery Personnel Dashboard
- **View Assigned Deliveries**: Display meal boxes and patient details.
- **Mark Deliveries Completed**: Update delivery status and add timestamps/notes.

## Technologies Used

### Frontend
- **Framework**: React.js (Vite)
- **UI Library**: Material-UI / Bootstrap
- **State Management**: Context API (React Context)
- **Routing**: React Router

### Backend
- **Framework**: Node.js with Express
- **Database**: MongoDB (Mongoose ODM)
- **Authentication**: JSON Web Tokens (JWT)

### Tools
- Postman for API testing
- VS Code for development

## Installation

### Prerequisites
- Node.js and npm
- MongoDB instance
- Git

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/Kritika-badule/Hospital-Food-Delivery-Management
   cd hospital-food-system
   ```

2. Install dependencies for the backend:
   ```bash
   cd backend
   npm install
   ```

3. Set up the `.env` file in the `backend` folder:
   ```env
   PORT=5000
   MONGO_URI=<Your MongoDB URI>
   JWT_SECRET=<Your JWT Secret>
   ```

4. Start the backend server:
   ```bash
   npm run dev
   ```

5. Install dependencies for the frontend:
   ```bash
   cd ../frontend
   npm install
   ```

6. Start the frontend development server:
   ```bash
   npm run dev
   ```

7. Access the application at `http://localhost:5173`.

## Project Structure

### Backend
```
/backend
├── server.js
├── /models
├── /routes
├── /controllers
├── /middleware
└── /config
```

### Frontend
```
/frontend
├── /src
    ├── /components
    ├── /pages
    ├── /hooks
    ├── /context
    ├── /utils
    ├── App.jsx
    ├── index.jsx
    └── index.css
```

## Usage

### Roles and Features
- **Manager**: Create diet charts, manage pantry, track preparation and delivery.
- **Inner Pantry Staff**: Update meal preparation status, manage deliveries.
- **Delivery Personnel**: Mark deliveries as completed.

### API Endpoints
Refer to the Postman collection for testing endpoints.

## Contributing
1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add feature"
   ```
4. Push to the branch:
   ```bash
   git push origin feature-name
   ```
5. Open a Pull Request.

