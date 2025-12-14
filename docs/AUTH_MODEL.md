# Auth & Authorization Model

## Authentication
- JWT-based authentication
- Access token only (no refresh token for simplicity)
- Passwords hashed with bcrypt

## Authorization
- Role-Based Access Control (RBAC)
- Roles: USER, ADMIN

### Rules
- USER:
  - View sweets
  - Search sweets
  - Purchase sweets
- ADMIN:
  - All USER permissions
  - Add/update/delete sweets
  - Restock inventory

Role stored in JWT payload.