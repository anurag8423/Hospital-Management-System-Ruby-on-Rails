# Hospital Management System

A comprehensive hospital management system with secure authentication, role-based authorization, and full CRUD operations for managing medical records, staff, and patients.

## Key Features
- Role-based access control (Admin, Doctor, Patient)
- Secure user authentication with Devise
- Authorization management with Pundit
- Patient registration and medical records management
- Doctor appointment scheduling system
- Staff management CRUD operations
- Medical inventory tracking
- Audit logging for sensitive operations

## Technologies Used
- Ruby 3.2.2
- Rails 7.0.8
- PostgreSQL 14+
- Devise (Authentication)
- Pundit (Authorization)
- Bootstrap 5 (Frontend)
- Hotwire (Turbo & Stimulus)

## Prerequisites

- Ruby 3.2.2
- Rails 7.0.8
- PostgreSQL 14+
- Node.js 16.x+
- Yarn 1.22.x+

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/anurag8423/Hospital-Management-System-Ruby-on-Rails.git
   cd Hospital-Management-System-Ruby-on-Rails
   
2. **Install dependencies**
   ```bash
   bundle install
   yarn install
   
3. **Database setup**
   ```bash
   rails db:create
   rails db:migrate
   rails db:seed

4. **Running the Application**
   ```bash
   rails server


Access the system at: [http://localhost:3000](http://localhost:3000)


## User Roles

| Role    | Permissions |
|---------|-------------|
| Admin   | Full system access, user management, role assignment |
| Doctor  | View/update patient records, manage appointments |
| Patient | View personal records, book appointments |
| Staff   | Manage inventory, handle registrations |



## CRUD Operations

Managed Entities:
- Patients
- Doctors
- Appointments
- Medical Records
- Prescriptions
- Inventory Items

Example Endpoints:
- `GET /patients` (Admin only)
- `POST /appointments` (Doctors & Patients)
- `PATCH /medical_records/:id` (Doctors only)
- `DELETE /users/:id` (Admin only)



## Security Practices
- Role-based access control
- Password encryption with bcrypt
- CSRF protection
- Session timeout after 30 minutes
- Audit trails for sensitive operations
- Regular dependency updates
