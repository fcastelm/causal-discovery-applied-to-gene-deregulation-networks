# Causal Discovery Applied to Gene Deregulation Networks

## Abstract

Causal discovery is a key tool for inferring cause-and-effect relationships from observational data, with relevant applications in cancer bioinformatics. This thesis evaluates the performance of a nonparametric causal discovery algorithm implemented in the `CChains` code, developed to infer gene deregulation networks from gene expression data. The first objective is to validate the method using synthetic data generated from known causal graphs, allowing a quantitative comparison between the inferred and original graphs. Performance metrics such as discovery fraction, structural similarity, and spurious-edge elimination fraction are used to assess the algorithm under various topological configurations. Subsequently, the method is applied to real gene expression data from normal and tumor tissue samples corresponding to prostate adenocarcinoma (PRAD), lung adenocarcinoma (LUAD), and lung squamous cell carcinoma (LUSC), retrieved from the TCGA database. Finally, genes with high structural relevance are identified in the resulting causal networks by applying centrality measures from graph theory. The results validate the proposed method under reasonable probabilistic assumptions and suggest a set of candidate genes potentially involved in cancer-associated gene regulation mechanisms.

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
├── docs/
│   └── thesis.pdf
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
