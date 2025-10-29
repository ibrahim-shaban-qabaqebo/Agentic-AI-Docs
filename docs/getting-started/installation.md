# Installation

This guide will help you install and set up Agentic AI in your environment.

## Prerequisites

Before installing Agentic AI, ensure you have:

- Python 3.10 or higher
- pip or uv package manager
- An API key (get one from [your dashboard](https://dashboard.agentic-ai.com))

## Installation Methods

### Using pip

```bash
pip install agentic-ai
```

### Using uv (Recommended)

```bash
uv pip install agentic-ai
```

### From Source

```bash
git clone https://github.com/YOUR_USERNAME/agentic-ai.git
cd agentic-ai
pip install -e .
```

## Verify Installation

After installation, verify that everything is working:

```bash
python -c "import agentic_ai; print(agentic_ai.__version__)"
```

You should see the version number printed.

## Next Steps

- [Quick Start Guide](quick-start.md) - Get up and running in 5 minutes
- [Configuration](configuration.md) - Configure your settings
