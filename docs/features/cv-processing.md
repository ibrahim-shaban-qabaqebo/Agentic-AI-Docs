# CV Processing

Agentic AI provides advanced CV/resume processing capabilities using state-of-the-art AI models.

## Features

- Automatic CV parsing
- Skills extraction
- Experience analysis
- Education detection
- Contact information extraction

## Usage

```python
from agentic_ai import CVProcessor

processor = CVProcessor(api_key="your-api-key")
result = processor.process("path/to/cv.pdf")

print(result.summary)
print(result.skills)
print(result.experience)
```
