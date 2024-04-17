# Backend - Hospital Management System

## Overview
This is the backend part of the Hospital Management System. It handles all the server-side logic and database interactions for managing patients, appointments, medical records, users, billing, pharmacy, lab tests, and notifications.

## Technology Stack
- **Node.js**: Server runtime environment.
- **Express**: Web application framework.
- **MongoDB/Mongoose**: Database management.
- **dotenv**: Environment variable management.

## Installation

1. Clone the repository:
git clone <https://github.com/eyosiasbitsu/HospitalManagementSystem.git>

2. Navigate to the backend directory:
cd backend

3. Install dependencies:
npm install express nodemon mongoose bcrypt bcryptjs dotenv mongodb


## Running the Server

- Start the server with:
npm start


## API Endpoints

### Patient Management
- `POST /patients`: Register a new patient.
- `GET /patients/{id}`: Retrieve a patient's details.
- `PUT /patients/{id}`: Update a patient's information.
- `DELETE /patients/{id}`: Delete a patient's record.

### Appointment Management
- `POST /appointments`: Create a new appointment.
- `GET /appointments/{id}`: Get details of a specific appointment.
- `PUT /appointments/{id}`: Update an existing appointment.
- `DELETE /appointments/{id}`: Cancel an appointment.

### Medical Records Management
- **GET /medicalRecords/{patientId}**: Retrieve medical records for a patient.
- **POST /medicalRecords**: Add new medical record entry.
- **PUT /medicalRecords/{recordId}**: Update a medical record entry.

### Administration Functions
- **POST /users**: Create new user account (for hospital staff).
- **GET /users/{id}**: Get user details.
- **PUT /users/{id}**: Update user information.
- **DELETE /users/{id}**: Deactivate a user account.

### Finance and Billing
- **GET /billing/{patientId}**: Retrieve billing information for a patient.
- **POST /billing**: Create a new billing record.
- **PUT /billing/{billId}**: Update billing information.

### Pharmacy Management
- **GET /pharmacy/medicines**: List all medicines.
- **POST /pharmacy/medicines**: Add new medicine to the store.
- **PUT /pharmacy/medicines/{medicineId}**: Update medicine details.
- **DELETE /pharmacy/medicines/{medicineId}**: Remove medicine from inventory.

### Lab Management
- **POST /labs/tests**: Request new lab tests.
- **GET /labs/results/{patientId}**: Retrieve lab results for a patient.

### Notifications and Alerts
- **POST /notifications**: Send out a notification.
- **GET /notifications/{userId}**: Retrieve notifications for a user.

## Directory Structure

- `src/`: Source code.
- `api/`: Controllers, routes, and middlewares.
- `config/`: Configuration files.
- `models/`: Database models.
- `services/`: Business logic.
- `utils/`: Utility functions.
- `test/`: Unit and integration tests.
- `.env`: Environment variables.
- `.gitignore`: Specifies intentionally untracked files.
- `server.js`: Entry point of the application.

## Testing

To run tests:
npm test