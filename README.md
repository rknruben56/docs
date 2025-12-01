# Docs

Miscellaneous docs about Ruben

## Resume

[Resume PDF](https://rknruben56.github.io/docs/RubenRodriguezResume.pdf)

LaTeX resume that automatically builds and deploys to GitHub Pages.

## Setup

### How It Works

When changes are pushed to the `main` branch:

1. GitHub Actions automatically compiles `resume/RubenRodriguezResume.tex` to PDF
2. The PDF is deployed to GitHub Pages

## Local Development

To compile the resume locally, you need a LaTeX distribution installed:

```bash
# On macOS with Homebrew
brew install --cask mactex

# Compile the PDF
cd resume
pdflatex RubenRodriguezResume.tex
```

## File Structure

```
.
├── .github/
│   └── workflows/
│       └── build-and-deploy.yml  # GitHub Actions workflow
├── resume/
│   └── RubenRodriguezResume.tex  # LaTeX source file
└── README.md                      # This file
```
