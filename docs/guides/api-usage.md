# API Usage Guide

Learn how to use the Agentic AI REST API effectively.

## Authentication

All API requests require authentication using your API key:

```bash
curl -H "Authorization: Bearer YOUR_API_KEY" \
  https://api.agentic-ai.com/v1/agents
```

## Making Requests

### Using cURL

```bash
curl -X POST https://api.agentic-ai.com/v1/agents \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "name": "my-agent",
    "model": "gpt-4",
    "instructions": "You are a helpful assistant"
  }'
```

### Using Python

```python
import requests

headers = {
    "Authorization": "Bearer YOUR_API_KEY",
    "Content-Type": "application/json"
}

response = requests.post(
    "https://api.agentic-ai.com/v1/agents",
    headers=headers,
    json={
        "name": "my-agent",
        "model": "gpt-4",
        "instructions": "You are a helpful assistant"
    }
)
```

### Using JavaScript

```javascript
const response = await fetch('https://api.agentic-ai.com/v1/agents', {
  method: 'POST',
  headers: {
    'Authorization': 'Bearer YOUR_API_KEY',
    'Content-Type': 'application/json'
  },
  body: JSON.stringify({
    name: 'my-agent',
    model: 'gpt-4',
    instructions: 'You are a helpful assistant'
  })
});
```

## Response Format

All API responses follow a consistent format:

```json
{
  "success": true,
  "data": {
    "id": "agent_123",
    "name": "my-agent",
    "created_at": "2024-01-01T00:00:00Z"
  },
  "error": null
}
```

## Error Handling

API errors follow this format:

```json
{
  "success": false,
  "data": null,
  "error": {
    "code": "INVALID_REQUEST",
    "message": "Invalid API key",
    "details": {}
  }
}
```

Common error codes:
- `INVALID_API_KEY`: Invalid or missing API key
- `RATE_LIMIT_EXCEEDED`: Too many requests
- `INVALID_REQUEST`: Malformed request
- `SERVER_ERROR`: Internal server error

## Rate Limits

- Free tier: 100 requests/hour
- Pro tier: 1000 requests/hour
- Enterprise: Custom limits

Rate limit headers:
```
X-RateLimit-Limit: 1000
X-RateLimit-Remaining: 999
X-RateLimit-Reset: 1609459200
```

## Pagination

List endpoints support pagination:

```bash
curl "https://api.agentic-ai.com/v1/agents?page=1&limit=10"
```

Response includes pagination metadata:

```json
{
  "data": [...],
  "pagination": {
    "page": 1,
    "limit": 10,
    "total": 100,
    "pages": 10
  }
}
```
