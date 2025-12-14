# TDD Test Plan (Backend)

## Auth Tests
- Register user (success)
- Register duplicate email (fail)
- Login valid credentials (success)
- Login invalid credentials (fail)
- JWT required for protected routes

## Role Tests
- USER cannot delete sweet
- ADMIN can delete sweet

## Sweets Tests
- Add sweet
- List sweets
- Search sweets by name/category/price
- Update sweet
- Delete sweet (ADMIN only)

## Inventory Tests
- Purchase decreases quantity
- Purchase fails if quantity = 0
- Restock increases quantity (ADMIN only)