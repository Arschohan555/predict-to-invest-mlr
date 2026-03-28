# notebook-to-pdf-1

AI-Powered Jupyter Notebook to PDF Converter using LangChain with Ollama.

## Features

- Converts `.ipynb` files to professional PDFs
- AI-powered notebook analysis using LangChain + Ollama
- Syntax highlighting for code cells
- Markdown rendering support
- Preserves code output formatting
- Multiple page size options (Letter, A4)

## Installation

```bash
uv pip install -e .
```

Or install dependencies manually:

```bash
uv pip install langchain langchain-ollama ollama nbformat nbconvert reportlab pygments
```

## Usage

```bash
uv run --active python nb2-pdf-agent.py <notebook-file.ipynb>
```

### Options

- Input notebook file (`.ipynb`)
- Output PDF is generated in the same directory

### Example

```bash
uv run --active python nb2-pdf-agent.py test.ipynb
```

## Requirements

- Python 3.11+
- Ollama running locally (for AI analysis)
- Required packages: langchain, langchain-ollama, ollama, nbformat, nbconvert, reportlab, pygments