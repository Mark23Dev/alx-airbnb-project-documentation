# Airbnb Clone Backend – Features and Functionalities

This document outlines the key features and functionalities of the backend system for the Airbnb Clone project.

---

##  Core Features

### 1. User Authentication & Management
- Register new users (guest or host)
- Secure login/logout with hashed passwords
- JWT-based session handling
- Role-based access (admin, host, guest)

### 2. Property Listing Management (Hosts)
- Add, edit, or delete property listings
- Upload property images
- Set pricing, availability, and amenities
- View and manage bookings for their property

### 3. Search and Filter (Guests)
- Search listings by location, price, amenities
- View property details and images
- Filter by availability and ratings

### 4. Booking System
- Book an available property
- Calendar integration for dates
- Booking history for users
- Automatic conflict checking

### 5. Payment Integration
- Choose payment method: Stripe, PayPal, Credit Card
- Generate invoice for bookings
- Payment status: pending, confirmed, failed

### 6. Reviews and Ratings
- Leave reviews for properties after stay
- Rate host and property
- Flag inappropriate content

### 7. Admin Features
- View all users and listings
- Ban users or remove listings
- View booking and transaction logs

---

##  System Functionalities

- RESTful API design
- Secure and scalable architecture
- PostgreSQL database with UUIDs and ENUM types
- Automated tests for critical endpoints
- Swagger/OpenAPI documentation

---

##  Visual Diagram

See the attached PNG diagram for a visual overview of all backend components and how they interact.

---

##  File Structure

