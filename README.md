# Causal Discovery Applied to Gene Deregulation Networks

This repository contains the English LaTeX manuscript and figure assets for a thesis on causal discovery in gene deregulation networks.

## Overview

- Thesis topic: causal discovery applied to cancer-related gene deregulation networks
- Format: LaTeX manuscript with local image assets
- Scope of this repository: source files for a public, GitHub-ready thesis layout

## Repository Structure

```text
.
├── README.md
├── .gitignore
├── manuscript/
│   └── thesis.tex
└── assets/
    └── images/
        └── *.jpg
```

## Compile Guidance

From the repository root, compile the manuscript by pointing your LaTeX toolchain to:

```text
manuscript/thesis.tex
```

Typical examples:

```bash
pdflatex manuscript/thesis.tex
```

or

```bash
latexmk -pdf manuscript/thesis.tex
```

The manuscript uses `\graphicspath` so image references resolve from `assets/images/` without rewriting every `\includegraphics` call.

If you want to publish a curated final PDF in the repository, place it at `docs/thesis.pdf` after building locally.
