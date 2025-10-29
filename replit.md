# Hospital Management System

## Overview
A comprehensive full-stack hospital management system built with Spring Boot (Java) backend and React frontend. The system supports multiple user roles with role-based access control and provides complete management of hospital operations.

## Architecture
- **Backend**: Spring Boot 3.1.5 with Java 19
- **Frontend**: React with Vite
- **Database**: H2 Database (configured for MySQL-compatible operations)
- **Authentication**: JWT-based authentication with role-based authorization
- **Security**: Spring Security with role-based access control

## User Roles
1. **ADMIN** - Full system access, manages all entities
2. **DOCTOR** - View patients, manage appointments, write prescriptions
3. **NURSE** - Monitor patients, assist doctors
4. **RECEPTIONIST** - Register patients, schedule appointments, manage billing
5. **PATIENT** - Book appointments, view medical records

## Features Implemented

### Core Features
- ✅ User authentication with JWT
- ✅ Role-based access control
- ✅ Patient management (CRUD operations)
- ✅ Doctor management with specializations
- ✅ Appointment scheduling with status tracking
- ✅ Billing and invoice management
- ✅ Department management
- ✅ Room management with availability status
- ✅ Staff management
- ✅ Dashboard with statistics and charts

### API Endpoints
- `/api/auth/*` - Authentication (login, register)
- `/api/patients/*` - Patient management
- `/api/doctors/*` - Doctor management
- `/api/appointments/*` - Appointment scheduling
- `/api/invoices/*` - Billing and payments
- `/api/departments/*` - Department management
- `/api/rooms/*` - Room management
- `/api/staff/*` - Staff management
- `/api/dashboard/*` - Dashboard statistics

## Tech Stack

### Backend
- Spring Boot 3.1.5
- Spring Security with JWT
- Spring Data JPA
- H2 Database
- Lombok
- Maven

### Frontend
- React 18
- React Router v6
- Axios for API calls
- Recharts for data visualization
- CSS3 for styling

## Demo Credentials
- **Admin**: username=`admin`, password=`admin123`
- **Doctor**: username=`drjohn`, password=`doctor123`
- **Nurse**: username=`nurse1`, password=`nurse123`
- **Receptionist**: username=`receptionist1`, password=`receptionist123`

## Project Structure
```
.
├── src/main/java/com/hospital/          # Backend Java source
│   ├── model/                            # Entity models
│   ├── repository/                       # Data repositories
│   ├── controller/                       # REST controllers
│   ├── security/                         # JWT & Security config
│   ├── config/                           # Application configuration
│   └── dto/                              # Data transfer objects
├── src/main/resources/
│   └── application.properties            # Application configuration
├── frontend/                             # React frontend
│   ├── src/
│   │   ├── api/                          # API configuration
│   │   ├── components/                   # React components
│   │   ├── pages/                        # Page components
│   │   └── context/                      # React context (Auth)
│   └── vite.config.js                    # Vite configuration
├── pom.xml                               # Maven dependencies
└── data/                                 # H2 database files

## Development Notes
- Backend runs on port 8080
- Frontend runs on port 5000
- H2 console available at /h2-console
- CORS configured for localhost:5000
- Sample data is auto-initialized on first run

## Recent Changes
- Initial project setup with Spring Boot and React
- Implemented complete entity model structure
- Created REST API endpoints for all features
- Built JWT authentication system
- Developed React frontend with routing
- Created dashboard with role-based views
- Set up patient management interface

## Next Steps (Future Enhancements)
- Add notification system (Email/In-app)
- Implement advanced search and filtering
- Add PDF export for reports and invoices
- Implement comprehensive audit logging
- Add dark/light mode theme
- Multi-language support (English/Arabic)
- File upload for medical documents
- Appointment calendar view
