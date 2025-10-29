# Quick Start

Get up and running with Agentic AI in just a few minutes.

## Step 1: Install Agentic AI

```bash
pip install agentic-ai
```

## Step 2: Set Your API Key

```bash
export AGENTIC_AI_API_KEY="your-api-key-here"
```

Or create a `.env` file:

```env
AGENTIC_AI_API_KEY=your-api-key-here
```

## Step 3: Create Your First Agent

```python
from agentic_ai import Agent

# Initialize your agent
agent = Agent(
    api_key="your-api-key-here",
    name="my-first-agent"
)

# Give it a task
response = agent.run("Analyze the weather and suggest activities")
print(response)
```

## Step 4: Process Your First CV

```python
from agentic_ai import CVProcessor

processor = CVProcessor(api_key="your-api-key-here")
result = processor.process("path/to/cv.pdf")
print(result.summary)
```

## What's Next?

- Learn about [configuration options](configuration.md)
- Explore [advanced features](../features/ai-agents.md)
- Check out [API documentation](../api/overview.md)
