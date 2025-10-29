# Basic Examples

Simple examples to get you started.

## Creating an Agent

```python
from agentic_ai import Agent

agent = Agent(api_key="your-key")
result = agent.run("Hello, world!")
print(result)
```

## Processing a CV

```python
from agentic_ai import CVProcessor

processor = CVProcessor(api_key="your-key")
result = processor.process("cv.pdf")
print(result.summary)
```
