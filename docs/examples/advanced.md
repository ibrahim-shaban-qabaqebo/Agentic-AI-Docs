# Advanced Examples

Complex use cases and patterns.

## Multi-Agent Workflow

```python
from agentic_ai import Agent, Workflow

researcher = Agent(name="researcher")
analyzer = Agent(name="analyzer")

workflow = Workflow([researcher, analyzer])
result = workflow.run("Research and analyze topic X")
```

## Batch Processing

```python
from agentic_ai import CVProcessor

processor = CVProcessor(api_key="your-key")
cvs = ["cv1.pdf", "cv2.pdf", "cv3.pdf"]

results = processor.batch_process(cvs)
for result in results:
    print(result.summary)
```
