# airbnb-clone-project

## Project Overview

The Airbnb Clone Project is a comprehensive, real-world application designed to simulate the development of a robust booking platform like Airbnb. It involves a deep dive into full-stack development, focusing on backend systems, database design, API development, and application security.

## Project Goals

To enhance my expertise in modern software development practices. These tasks includes:

- Master collaborative team workflows using GitHub.
- Deepen my understanding of backend architecture and database design principles.
- Implement advanced security measures for API development.
- Gain proficiency in designing and managing CI/CD pipelines for efficient deployment.
- Strengthen my ability to document and plan complex software projects effectively.
- Develop an understanding of integrating technologies like Django, MySQL, and GraphQL in a unified ecosystem.

## Team Roles

**Backend Developer**:
Responsible for implementing API endpoints, database schemas, and business logic.

**Database Administrator**:
Manages database design, indexing, and optimizations.

**DevOps Engineer**:
Handles deployment, monitoring, and scaling of the backend services.

**QA Engineer**:
Ensures the backend functionalities are thoroughly tested and meet quality standards.

## Technology Stack

| **Technology**        | **Description**                                                                       |
| --------------------- | ------------------------------------------------------------------------------------- |
| Django                | A Python web framework used for building the RESTful API.                             |
| Django REST Framework | Flexible toolkit for creating and managing RESTful APIs.                              |
| PostgreSQL            | A relational database system used for data storage.                                   |
| GraphQL               | Allows for flexible and efficient querying of data.                                   |
| Celery                | For handling asynchronous tasks such as sending notifications or processing payments. |
| Redis                 | Used for caching and session management.                                              |
| Docker                | Containerization tool for consistent development and deployment environments.         |
| CI/CD Pipelines       | Automated pipelines for testing and deploying code changes.                           |

## Database Design

| **Entity** | **Fields**                                                         |
| ---------- | ------------------------------------------------------------------ |
| **Users**  | user_id, first_name, last_name, email_address, password.           |
| Properties | property_id, physical_address, property_description, property_host |
| Bookings   | booking_id, booking_date, booking_price                            |
| Payments   | payment_id, payment_reference, payment_status, payment_method      |
| Reviews    | review_id, review_message, reivew_rating                           |

A **user** can list multiple **properties**, **book** multiple properties and multiple **users** can interact about the **booking** of a **property**.
A **property** belongs to a user and can be **booked** by multiple users.
A **booking** belongs to a **property** and a property can have multiple **bookings**.
A **payment** can be made for a **booking** by a **user** and a **user** will recieve payment for a **booking** of their listed **property**
A **review** can be submitted by a **user** for a **property** and a **review** can be submitted by a host(**user**) on a **user** who **booked** their **property**.
