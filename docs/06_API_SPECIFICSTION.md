# LOKA API Specification

Version: v1.0

Architecture: REST API

Format: JSON

Authentication: JWT

---

# Base URL

Development

/api/v1

Production

/api/v1

---

# Authentication

## POST /auth/register

Description:

Register a new user.

Request

{
  "full_name": "John Doe",
  "email": "john@email.com",
  "password": "password123"
}

Response

{
  "success": true,
  "message": "User registered successfully."
}

---

## POST /auth/login

Description

User login.

Request

{
  "email":"john@email.com",
  "password":"password123"
}

Response

{
  "token":"JWT_TOKEN"
}

---

# Trips

## GET /trips

Description

Get all trips.

---

## GET /trips/{id}

Description

Get trip detail.

---

## POST /trips

Description

Create new trip.

Request

{
  "origin":"Yogyakarta",
  "destination":"Bandung",
  "departure_date":"2026-08-01",
  "return_date":"2026-08-03",
  "budget":1500000
}

Response

{
  "trip_id":"UUID"
}

---

## PUT /trips/{id}

Update trip.

---

## DELETE /trips/{id}

Delete trip.

---

# Budget

## POST /budget/calculate

Description

Calculate estimated travel budget.

Response

{
  "ticket":350000,
  "hotel":500000,
  "food":300000,
  "transport":150000,
  "tourism":200000,
  "total":1500000
}

---

# AI

## POST /ai/chat

Description

Chat with RAILA.

Request

{
  "message":"Saya ingin liburan ke Bandung naik kereta."
}

Response

{
  "reply":"Tentu! Berikut itinerary yang saya rekomendasikan..."
}

---

# Saved Trips

GET /saved-trips

POST /saved-trips

DELETE /saved-trips/{id}

---

# Reminder

GET /reminders

POST /reminders

DELETE /reminders/{id}

---

# User Profile

GET /profile

PUT /profile

DELETE /profile

---

Status

Draft v1.0
