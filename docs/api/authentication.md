# Authentication

All API requests require authentication using your API key.

## API Key

Obtain your API key from the [dashboard](https://dashboard.agentic-ai.com).

## Usage

Include your API key in the Authorization header:

```bash
Authorization: Bearer YOUR_API_KEY
```

## Security

- Never commit API keys to version control
- Use environment variables for storage
- Rotate keys regularly
- Use different keys for different environments
