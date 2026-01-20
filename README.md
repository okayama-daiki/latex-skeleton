# latex-skeleton

Minimal LaTeX skeletons for writing reports and slides in **Japanese**.

## Overview

This repository provides minimal yet sufficient LaTeX starter files for Japanese academic documents.

- `report.tex`  
  A minimal report template based on the `jlreq` article class, which is designed to meet the requirements of Japanese text layout.

- `slides.tex`  
  A Beamer slide template using the Metropolis theme (16:9).

- `figures/` and `references.bib`  
  Example files for figures and bibliography management with BibLaTeX.

- `.latexmkrc`  
  Build configuration for upLaTeX, BibLaTeX, and latexmk.

A Dev Container configuration is also included for portability.

## Requirements

If you do not have TeX Live installed locally, the following environment is required:

- [Docker](https://www.docker.com/)  
  A platform for building and running containerized applications.

- [Zed](https://zed.dev)  
  A fast, minimal code editor. Configuration files for Zed are included.

This templates can also be built in any Dev Container–compatible environment.

## Quick start

Build everything (resume and slides):

1. Open the Dev Container (or install TeX Live locally)
2. Run:
    ```bash
    latexmk resume.tex
    # or
    latexmk slides.tex
    ```
3. Output PDFs are written to `dist/`, and intermediate files to `.tex/` (as configured in .latexmkrc)

Clean artifacts:

```bash
latexmk -C
rm -rf dist .tex
```

## Credit

- Maintainer: [Daiki Okayama](https://github.com/okayama-daiki)
