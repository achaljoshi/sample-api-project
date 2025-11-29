# API Documentation

## Base URL
`https://dummy-json.mock.beeceptor.com`

## Endpoints

### GET /posts
List all available blog posts

**Response:** Array of post objects

**Example Request:**
```
GET https://dummy-json.mock.beeceptor.com/posts
```

**Example Response (200):**
```json
[
  {
    "userId": 1,
    "id": 1,
    "title": "Introduction to Artificial Intelligence",
    "body": "Learn the basics...",
    "link": "https://example.com/article1",
    "comment_count": 8
  }
]
```

### GET /posts/{post_id}
Retrieve a post by ID

**Parameters:**
- `post_id` (path, required): Integer ID of the post

**Example Request:**
```
GET https://dummy-json.mock.beeceptor.com/posts/1
```

**Example Response (200):**
```json
{
  "userId": 1,
  "id": 1,
  "title": "Introduction to Artificial Intelligence",
  "body": "Learn the basics...",
  "link": "https://example.com/article1",
  "comment_count": 8
}
```

### GET /comments
List all blog comments

**Example Request:**
```
GET https://dummy-json.mock.beeceptor.com/comments
```

### GET /countries
List all countries

**Example Request:**
```
GET https://dummy-json.mock.beeceptor.com/countries
```

### GET /continents
List all continents with detailed information

**Example Request:**
```
GET https://dummy-json.mock.beeceptor.com/continents
```

## HTTP Methods Supported

- **GET** - Retrieve resources
- **POST** - Create new resources (schema defined for future use)
- **PUT** - Full update (schema defined for future use)
- **PATCH** - Partial update (schema defined for future use)
- **DELETE** - Delete resources (schema defined for future use)

## Error Responses

All error responses follow RFC 7807 Problem Details format:

```json
{
  "type": "/problem-details/types/error-type",
  "title": "Error Title",
  "status": 400,
  "detail": "Detailed error message",
  "instance": "/path/to/resource"
}
```

## Status Codes

- `200` - Success
- `201` - Created
- `204` - No Content
- `400` - Bad Request
- `401` - Unauthorized
- `403` - Forbidden
- `404` - Not Found
- `500` - Internal Server Error

