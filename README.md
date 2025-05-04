# Airbnb Clone Project

## Overview

The Airbnb Clone Project is a full-stack web development initiative that simulates the creation of a real-world booking platform similar to Airbnb. This project focuses on backend system architecture, relational database design, secure API development, and CI/CD integration. It provides hands-on experience in building scalable, maintainable, and secure backend services, empowering learners to apply industry best practices in a collaborative development environment.

## Project Goals

* Develop a fully functional backend for an Airbnb-like platform.
* Design and implement a robust relational database schema.
* Build secure and scalable APIs using modern frameworks.
* Integrate CI/CD pipelines to automate testing and deployment.
* Promote collaborative workflows through GitHub-based team development.
* Understand and apply backend security best practices.

## Tech Stack  
- Django (Backend framework)  
- PostgreSQL (Database)  
- GraphQL (API queries)  
- Docker (Containerization)  
- GitHub Actions (CI/CD)

## Team Roles

- **Backend Developer**: Designs and implements server-side logic, APIs, and integration with the database using Django. Ensures robust performance and security of backend services.

- **Database Administrator (DBA)**: Defines the database schema, optimizes query performance, manages migrations, and ensures data integrity and backups using PostgreSQL.

- **Frontend Developer** *(optional role if integrating frontend)*: Develops the UI/UX components to interact with backend services. Works closely with backend via REST or GraphQL APIs.

- **DevOps Engineer**: Sets up and maintains CI/CD pipelines using tools like GitHub Actions and Docker. Automates testing, deployment, and monitors infrastructure.

- **QA Engineer**: Designs test plans, executes manual/automated tests, and ensures that all features meet functional and performance requirements.

- **Project Manager**: Coordinates project activities, sets timelines, and facilitates communication between team members. Ensures that the project is delivered on time and meets quality standards.

- **Security Specialist** *(shared or rotating role)*: Ensures secure data access, implements authentication/authorization mechanisms, and addresses potential vulnerabilities in the system. 

## Technology Stack

* **Django**: A high-level Python web framework used for rapid API development.
* **PostgreSQL**: A powerful open-source relational database system for managing structured data.
* **GraphQL**: A flexible query language for APIs that allows clients to request exactly the data they need.
* **Docker**: Used for containerizing the application to ensure consistency across different environments.
* **GitHub Actions**: CI/CD automation tool used to streamline development workflows and deployments.
* **Python**: Main backend language for business logic and data processing.
* **Git**: Version control system for collaborative code management.

## Database Design

### Key Entities:

* **Users**

  * `id`, `username`, `email`, `password_hash`, `role`
* **Properties**

  * `id`, `owner_id`, `title`, `description`, `price_per_night`
* **Bookings**

  * `id`, `user_id`, `property_id`, `start_date`, `end_date`
* **Reviews**

  * `id`, `user_id`, `property_id`, `rating`, `comment`
* **Payments**

  * `id`, `booking_id`, `amount`, `status`, `transaction_date`

### Relationships:

* A user can own multiple properties.
* A user can make multiple bookings.
* A booking is linked to one property and one user.
* A property can have multiple reviews.
* A booking has one payment.

## Feature Breakdown

* **User Management**: Registration, login, profile management, and role-based access.
* **Property Management**: List, update, and delete properties. View property details.
* **Booking System**: Book properties for specific dates, check availability, cancel bookings.
* **Reviews**: Users can leave ratings and comments on properties they’ve booked.
* **Payment Processing**: Simulate or integrate payment system for confirmed bookings.