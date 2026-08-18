# GPS Tech Doc

Sphinx-based technical documentation for the GPS Tech Doc project, covering High-Level Design (HLD) and Low-Level Design (LLD). Built with the Read the Docs theme.

## Prerequisites

- Python 3.x
- pip

## Installation

Install Sphinx and the Read the Docs theme:

```bash
pip install sphinx sphinx-rtd-theme
```

## Building the Documentation

All commands are run from inside the `docs` folder:

```bash
cd docs
```

### Windows

```bash
.\make.bat html
```

### Linux / macOS

```bash
make html
```

The generated HTML pages are written to `build/html/`.

## Preview

Open the generated site in a browser:

```bash
build\html\index.html
```

## Cleaning Build Output

Remove the generated files:

### Windows

```bash
.\make.bat clean
```

### Linux / macOS

```bash
make clean
```

## Project Structure

```
docs/
├── Makefile              # Makefile for Linux/macOS builds
├── make.bat              # Batch file for Windows builds
├── build/                # Generated output (created at build time)
└── source/
    ├── conf.py           # Sphinx configuration
    ├── index.rst         # Main entry point
    ├── overview.rst      # Project overview
    ├── HLD/              # High-Level Design documents
    ├── LLD/              # Low-Level Design documents
    ├── _static/          # Static assets (CSS, images)
    └── _templates/       # Custom HTML templates
```

## Extensions Used

- `sphinx.ext.autodoc` — automatically generate API documentation from docstrings
- `sphinx.ext.napoleon` — support for NumPy/Google style docstrings
- `sphinx.ext.viewcode` — add links to source code
- `sphinx.ext.autosectionlabel` — allow references to sections by label
