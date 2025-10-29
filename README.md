# Agentic AI Documentation

Professional documentation site built with MkDocs and Material theme, deployed to GitHub Pages.

## Features

- 🎨 Modern Material Design theme
- 📱 Fully responsive
- 🔍 Built-in search functionality
- 🌓 Dark/Light mode toggle
- ⚡ Fast page loads
- 📚 Automatic deployment via GitHub Actions

## Local Development

### Prerequisites

- Python 3.10 or higher
- [uv](https://github.com/astral-sh/uv) package manager

### Setup

1. Install dependencies:

```bash
uv pip install -e .
```

Or using pip:

```bash
pip install mkdocs-material mkdocs-minify-plugin
```

2. Start the development server:

```bash
mkdocs serve
```

3. Open `http://localhost:8000` in your browser

### Building

Build the static site:

```bash
mkdocs build
```

The site will be generated in the `site/` directory.

## Deployment

This documentation is automatically deployed to GitHub Pages via GitHub Actions when changes are pushed to the `main` or `master` branch.

### Manual Deployment

1. Configure GitHub Pages:
   - Go to repository Settings → Pages
   - Source: GitHub Actions

2. Push to trigger deployment:

```bash
git add .
git commit -m "Update documentation"
git push origin main
```

### Custom Domain

To use a custom domain:

1. Add a `CNAME` file to the `docs/` directory with your domain
2. Configure DNS settings in your domain provider
3. Update `site_url` in `mkdocs.yml`

## Project Structure

```
.
├── docs/              # Documentation source files
│   ├── index.md      # Home page
│   ├── getting-started/
│   ├── guides/
│   ├── features/
│   └── ...
├── mkdocs.yml        # MkDocs configuration
├── pyproject.toml    # Python dependencies
└── .github/
    └── workflows/
        └── deploy.yml  # GitHub Actions workflow
```

## Configuration

Edit `mkdocs.yml` to customize:

- Site name and description
- Navigation structure
- Theme settings
- Plugins and extensions

## Contributing

1. Create a new branch
2. Make your changes
3. Test locally with `mkdocs serve`
4. Submit a pull request

## License

MIT License - see LICENSE file for details
