# Project Overview
    The backend for the Airbnb Clone project is designed to provide a robust and scalable foundation for managing user interactions, property listings, bookings, and payments. This backend will support various functionalities required to mimic the core features of Airbnb, ensuring a smooth experience for users and hosts.

# Project Goals
    User Management: Implement a secure system for user registration, authentication, and profile management.
    Property Management: Develop features for property listing creation, updates, and retrieval.
    Booking System: Create a booking mechanism for users to reserve properties and manage booking details.
    Payment Processing: Integrate a payment system to handle transactions and record payment details.
    Review System: Allow users to leave reviews and ratings for properties.
    Data Optimization: Ensure efficient data retrieval and storage through database optimizations.

# Team Roles and Responsibilities

    Backend Developer: Responsible for implementing API endpoints, database schemas, and business logic.
    Database Administrator: Manages database design, indexing, and optimizations.
    DevOps Engineer: Handles deployment, monitoring, and scaling of the backend services.
    QA Engineer: Ensures the backend functionalities are thoroughly tested and meet quality standards.


# Tech Stack

    Django: A high-level Python web framework used for building the RESTful API.
    Django REST Framework: Provides tools for creating and managing RESTful APIs.
    PostgreSQL: A powerful relational database used for data storage.
    GraphQL: Allows for flexible and efficient querying of data.
    Celery: For handling asynchronous tasks such as sending notifications or processing payments.
    Redis: Used for caching and session management.
    Docker: Containerization tool for consistent development and deployment environments.
    CI/CD Pipelines: Automated pipelines for testing and deploying code changes.

# Database Design

    Users
        A user can own multiple properties (if a host).
        A user can make multiple bookings (if a guest).
        A user can write multiple reviews.

    Properties
        A property belongs to one user (the host).
        A property can have multiple bookings.
        A property can have multiple reviews.

    Bookings
        A booking belongs to one user (the guest).
        A booking belongs to one property.
        A booking can have one payment associated.

    Payments
        A payment is associated with one booking.
        Multiple payments can be made by a user(if a user has multiple bookings).
        A payment is associated to a specific property.

    Reviews
        A review belongs to one user (the reviewer).
        A review belongs to one property.
        A review references a single booking.
        

