# Backend Rules

## General Principles

- REST API only
- JSON response only
- JWT Authentication
- UUID as Primary Key
- UTC Timestamp
- Soft Delete where applicable

---

## API Standards

- Use nouns for endpoints
- Use HTTP status codes correctly
- Validate every request
- Never expose sensitive data
- Return consistent response format

---

## Error Response

{
  "success": false,
  "message": "Validation failed."
}

---

## Success Response

{
  "success": true,
  "data": {}
}
