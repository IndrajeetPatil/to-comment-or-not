# To Comment or Not To Comment

This presentation summarizes my understanding of best practices for code
comments in software development.

The slides can be seen at:
<https://indrajeetpatil.github.io/to-comment-or-not/>

[![introductory slide](media/pipe.jpg)](https://indrajeetpatil.github.io/to-comment-or-not/)

# Development

This project uses Python 3.13+ with [uv](https://docs.astral.sh/uv/) for dependency management, [Quarto](https://quarto.org/) for rendering slides, and [just](https://github.com/casey/just) as a command runner.

## Prerequisites

```bash
# Install just (macOS)
brew install just
```

## Setup

```bash
# Install dependencies
just install

# Or update to latest versions
just update
```

## Common Commands

```bash
just help      # Show all available commands
just render    # Render slides to HTML
just preview   # Live preview with auto-reload
just open      # Open rendered slides in browser
just clean     # Remove generated files
just check     # Check Quarto and Python setup
just           # Install, render, and open slides (default)
```

# Feedback

I'd love to hear thoughts and comments in
[the issue tracker](https://github.com/IndrajeetPatil/to-comment-or-not/issues).

# Code of Conduct

Please note that the to-comment-or-not project is released with a
[Contributor Code of Conduct](https://www.contributor-covenant.org/version/3/0/code_of_conduct/).
By contributing to this project, you agree to abide by its terms.
