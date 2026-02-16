# API Reference

## Endpoints

### GET /api/health

Health check endpoint.

**Response:**
```json
{
  "status": "ok",
  "timestamp": "2024-01-01T00:00:00Z"
}
```

### GET /api/items

Retrieve all items.

**Response:**
```json
{
  "items": [
    { "id": 1, "name": "Item 1" },
    { "id": 2, "name": "Item 2" }
  ]
}
```

### POST /api/items

Create a new item.

**Request Body:**
```json
{
  "name": "New Item"
}
```

**Response:**
```json
{
  "id": 3,
  "name": "New Item",
  "created": "2024-01-01T00:00:00Z"
}
```

### DELETE /api/items/:id

Delete an item by ID.

**Response:**
```json
{
  "message": "Item deleted successfully"
}
```
