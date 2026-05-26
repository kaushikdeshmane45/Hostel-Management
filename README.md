# Hostel Management System

## Overview

The Hostel Management System is a web-based application developed using the Django framework to simplify hostel administration and student management. The system helps wardens and administrators manage student records, room allocation, complaints, fee tracking, and notices from a centralized dashboard.

This project is designed to reduce manual work, improve data organization, and streamline hostel operations.

---

# Features

## Student Management

* Add, update, and delete student records
* Store student details such as:

  * Name
  * Email
  * Phone number
  * Address
  * College and course details
* Upload student photo and ID proof
* Assign students to hostel rooms

## Room Management

* Add and manage hostel rooms
* Track:

  * Room number
  * Room type
  * Floor number
  * Total beds
  * Available beds
  * Room rent
* Upload room images

## Complaint Management

* Students can submit complaints
* Admin can track complaint status
* Complaint records include:

  * Title
  * Description
  * Status
  * Date

## Fee Management

* Maintain hostel fee records
* Track:

  * Monthly payments
  * Amount paid
  * Payment status
  * Payment date

## Notice Board

* Add and publish notices for students
* Display important hostel announcements

## Authentication

* Separate management for students and wardens/admin
* Login-based access control

---

# Technologies Used

## Frontend

* HTML
* CSS
* Bootstrap

## Backend

* Python
* Django

## Database

* SQLite3

## Media Handling

* Django Media Files

---

# Project Structure

```bash
Hostel_Management-main/
│
├── accounts/            # Authentication and admin-related modules
├── complaints/          # Complaint management module
├── fees/                # Fee management module
├── hostel_management/   # Main project settings and configuration
├── notice/              # Notice board module
├── rooms/               # Room management module
├── students/            # Student management module
├── templates/           # HTML templates
├── media/               # Uploaded images and documents
├── manage.py
```

---

# Installation Guide

## 1. Clone the Repository

```bash
git clone https://github.com/your-username/hostel-management-system.git
cd hostel-management-system
```

## 2. Create Virtual Environment

```bash
python -m venv venv
```

## 3. Activate Virtual Environment

### Windows

```bash
venv\Scripts\activate
```

### Linux/Mac

```bash
source venv/bin/activate
```

## 4. Install Dependencies

```bash
pip install django pillow
```

## 5. Run Migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

## 6. Create Superuser

```bash
python manage.py createsuperuser
```

## 7. Start Development Server

```bash
python manage.py runserver
```

## 8. Open in Browser

```bash
http://127.0.0.1:8000/
```

---

# Database Models

## Student Model

Stores student-related information including personal details, room allocation, and uploaded documents.

## Room Model

Maintains room details such as room number, bed capacity, rent, and availability.

## Complaint Model

Tracks complaints submitted by students along with their status.

## Fee Model

Handles hostel fee payments and payment tracking.

## Notice Model

Stores hostel notices and announcements.

---

# Future Improvements

* Online fee payment integration
* Email notification system
* QR-based hostel entry system
* Attendance management
* Student dashboard analytics
* Role-based authentication system
* Responsive mobile application

---

# Learning Outcomes

Through this project, the following concepts were implemented and learned:

* Django project structure
* CRUD operations
* Database relationships using Django ORM
* File and image uploads
* Authentication and authorization
* Dynamic template rendering
* Backend development using Python
* Database integration with SQLite

---

# Conclusion

The Hostel Management System provides a practical solution for digitizing hostel administration. It minimizes paperwork, improves efficiency, and enables better management of students, rooms, complaints, and fees through an easy-to-use web interface.

This project demonstrates full-stack web development skills using Django and showcases practical implementation of database-driven web applications.
