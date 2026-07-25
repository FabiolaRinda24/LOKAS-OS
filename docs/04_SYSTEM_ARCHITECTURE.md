# LOKA SYSTEM ARCHITECTURE

## Overview

LOKA adalah aplikasi AI Train Trip Planner yang dibangun dengan arsitektur modern berbasis cloud dan AI.

---

# High Level Architecture

User

↓

Frontend (Web / Mobile)

↓

Backend API

↓

AI Engine (RAILA)

↓

Database

↓

External Services

---

# Frontend

Platform:

- Web Application
- Mobile Application (Future)

Technology:

- React
- Next.js
- Tailwind CSS

Responsibilities:

- User Interface
- Authentication
- Dashboard
- AI Chat
- Trip Planner

---

# Backend

Technology:

- FastAPI
- Python

Responsibilities:

- Business Logic
- Authentication
- Trip Management
- Budget Calculation
- AI Integration

---

# AI Engine (RAILA)

Model:

- OpenAI GPT
- Future Local AI Model

Responsibilities:

- AI Chat
- Travel Recommendation
- Budget Advice
- Itinerary Generation
- Trip Optimization

---

# Database

Primary Database:

- PostgreSQL

Cache:

- Redis (Future)

Storage:

- Cloud Storage

---

# External Services

- KAI Ticket API (Future)
- Google Maps API
- Weather API
- Hotel API (Future)
- Tourism API (Future)

---

# Authentication

- Email Login
- Google Login
- Future: Apple Login

---

# Security

- HTTPS
- JWT Authentication
- Password Hashing
- Environment Variables
- Rate Limiting

---

# Deployment

Frontend

↓

Vercel

Backend

↓

Railway / Render

Database

↓

Supabase PostgreSQL

Storage

↓

Cloud Storage

---

# Version 1.0 Stack

Frontend:
- Next.js

Backend:
- FastAPI

Database:
- PostgreSQL

AI:
- OpenAI API

Hosting:
- Vercel
- Railway

Version:
v1.0 MVP
