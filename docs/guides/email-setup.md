# Email Setup Guide

Learn how to configure and use email functionality with Agentic AI.

## Overview

Agentic AI provides powerful email automation capabilities that allow you to send, receive, and process emails programmatically.

## Configuration

### Gmail Setup

1. Enable IMAP in your Gmail settings
2. Generate an App Password:
   - Go to Google Account → Security
   - Enable 2-Step Verification
   - Generate App Password

```python
from agentic_ai import EmailClient

client = EmailClient(
    provider="gmail",
    email="your-email@gmail.com",
    app_password="your-app-password"
)
```

### SMTP Setup

```python
client = EmailClient(
    provider="smtp",
    smtp_server="smtp.gmail.com",
    smtp_port=587,
    username="your-email@gmail.com",
    password="your-password"
)
```

## Usage Examples

### Sending Emails

```python
client.send_email(
    to="recipient@example.com",
    subject="Hello from Agentic AI",
    body="This is an automated email."
)
```

### Receiving Emails

```python
emails = client.fetch_emails(max_results=10)
for email in emails:
    print(f"From: {email.from_address}")
    print(f"Subject: {email.subject}")
    print(f"Body: {email.body}")
```

### Email Processing with AI

```python
from agentic_ai import EmailProcessor

processor = EmailProcessor(api_key="your-api-key")
emails = client.fetch_emails()

for email in emails:
    # Analyze email content
    analysis = processor.analyze(email)
    
    # Generate response
    if analysis.needs_response:
        response = processor.generate_response(email)
        client.send_email(
            to=email.from_address,
            subject=f"Re: {email.subject}",
            body=response
        )
```

## Best Practices

1. **Use App Passwords**: Never use your main account password
2. **Rate Limiting**: Respect email provider rate limits
3. **Error Handling**: Always handle connection errors gracefully
4. **Security**: Store credentials securely using environment variables

## Troubleshooting

### Connection Issues

- Verify your credentials
- Check firewall settings
- Ensure IMAP/SMTP is enabled

### Authentication Errors

- Regenerate App Password
- Check 2FA settings
- Verify account permissions
