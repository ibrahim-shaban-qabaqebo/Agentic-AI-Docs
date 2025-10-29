# Configuration

Configure Agentic AI to match your needs and environment.

## Environment Variables

Set the following environment variables:

```bash
export AGENTIC_AI_API_KEY="your-api-key-here"
export AGENTIC_AI_BASE_URL="https://api.agentic-ai.com"
export AGENTIC_AI_TIMEOUT=30
```

## Configuration File

Create a `config.yaml` file:

```yaml
api:
  key: "${AGENTIC_AI_API_KEY}"
  base_url: "https://api.agentic-ai.com"
  timeout: 30

agents:
  default_model: "gpt-4"
  max_iterations: 10
  temperature: 0.7

cv_processing:
  enable_ocr: true
  language: "en"
  output_format: "json"
```

## Python Configuration

```python
from agentic_ai import configure

configure(
    api_key="your-api-key",
    base_url="https://api.agentic-ai.com",
    timeout=30,
    default_model="gpt-4"
)
```

## Settings

### API Settings

- `api_key`: Your API key (required)
- `base_url`: API endpoint URL
- `timeout`: Request timeout in seconds

### Agent Settings

- `default_model`: Default AI model to use
- `max_iterations`: Maximum agent iterations
- `temperature`: Model temperature (0-2)

### CV Processing Settings

- `enable_ocr`: Enable OCR for scanned documents
- `language`: Document language
- `output_format`: Output format (json, xml, markdown)
