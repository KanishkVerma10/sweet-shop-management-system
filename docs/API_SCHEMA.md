# API Schema – Sweet Shop Management System

Base URL: /api

## Auth
POST /auth/register
POST /auth/login

## Users
User:
- id (uuid)
- email
- passwordHash
- role: USER | ADMIN
- createdAt

## Sweets
Sweet:
- id (uuid)
- name
- category
- price
- quantity
- createdAt
- updatedAt

### Endpoints (JWT Protected)
POST   /sweets
GET    /sweets
GET    /sweets/search?name=&category=&minPrice=&maxPrice=
PUT    /sweets/{id}
DELETE /sweets/{id} (ADMIN)

## Inventory
POST /sweets/{id}/purchase
POST /sweets/{id}/restock (ADMIN)