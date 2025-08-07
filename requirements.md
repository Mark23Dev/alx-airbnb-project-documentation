# Backend Feature Requirements – ALX Airbnb Clone

This document outlines the **technical and functional requirements** for the key backend features of the Airbnb clone project. The features covered include:

1. User Authentication
2. Property Management
3. Booking System

---

## 1. User Authentication

### Functional Requirements:
- Users must be able to register, log in, and log out securely.
- Passwords must be hashed before storage.
- Authentication should use token-based (JWT) sessions.
- Only verified users can list properties or make bookings.

### API Endpoints:

#### POST `/api/v1/auth/register`
- **Description:** Register a new user
- **Input:**  
  ```json
  {
    "username": "johndoe",
    "email": "johndoe@example.com",
    "password": "SecurePass123"
  }

## 2. Property Management

### Functional Requirements
- Users (Hosts) can list new properties for rent.
- Hosts can edit or delete their listed properties.
- All users can view available properties.
- The system should store and retrieve property data including images, description, location, availability, and pricing.

### Technical Requirements

#### API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/api/properties/` | Create a new property listing |
| `GET` | `/api/properties/` | List all properties |
| `GET` | `/api/properties/{id}/` | Retrieve a single property by ID |
| `PUT` | `/api/properties/{id}/` | Update a property listing |
| `DELETE` | `/api/properties/{id}/` | Delete a property listing |

#### Input Specifications (for `POST` and `PUT`)

```json
{
  "title": "Cozy Studio Apartment",
  "description": "Fully furnished, near the beach.",
  "location": "Mombasa, Kenya",
  "price_per_night": 45.00,
  "available_from": "2025-09-01",
  "available_to": "2025-12-31",
  "images": ["image1.jpg", "image2.jpg"]
}