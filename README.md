# Library Management System

A web-based Library Management System built with Django and MySQL for managing library operations including book loans, reservations, member management, and staff administration.
<img width="1353" height="777" alt="Image" src="https://github.com/user-attachments/assets/3e063bf2-ac27-47f4-b067-1b2506dbd7e9" />

## Features

### Core Functionality
- **User Authentication**: Separate login systems for members and staff
- **Book Management**: Add, edit, delete, and browse books with ISBN tracking
- **Loan System**: Borrow and return books with due date tracking and fine calculation
- **Reservation System**: Reserve books with status management (pending/confirmed/cancelled)
- **Member Management**: Register, view, and remove library members
- **Staff Management**: Register, view, and resign staff members
- **Role-based Access**: Staff and admin have access to management features; members can view and manage their own loans and reservations

### User Roles
- **Members**: Browse books, borrow/return books, manage reservations
- **Staff**: Manage loans, reservations, and member accounts
- **Administrators**: Full system access including staff management

## Tech Stack

- **Backend**: Django 4.2+
- **Frontend**: Django Templates
- **Database**: MySQL

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/TaigaVanilla/library-management-system.git
   cd library-management-system
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Environment Configuration**
   Create a `.env` file in the project root with the following variables:
   ```env
   SECRET_KEY=your-secret-key-here
   DB_NAME=library_db
   DB_USER=your_db_user
   DB_PASSWORD=your_db_password
   DB_HOST=localhost
   DB_PORT=3306
   ```

4. **Run migrations**
   ```bash
   python manage.py migrate
   ```

5. **Create superuser (optional)**
   ```bash
   python manage.py createsuperuser
   ```

6. **Run the development server**
   ```bash
   python manage.py runserver
   ```
