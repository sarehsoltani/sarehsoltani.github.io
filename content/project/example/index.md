---
title: Example Project
summary: scGPT-based Single-Cell RNA-seq Immune Cell Annotation
tags:
  - Deep Learning
date: '2016-04-27T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:
  - icon: twitter
    icon_pack: fab
    name: Follow
    url: https://twitter.com/georgecushen
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---

Leveraging scVI—a generative variational auto-encoder designed for single-cell RNA-seq—I processed ~14k peripheral-blood cells (16k genes) from patients spanning mild to severe respiratory infection. After stringent QC, normalization, and feature selection, scVI learned a 30-D latent space that accounts for UMI over-dispersion, zero inflation, and donor-specific batch effects, enabling unbiased cross-patient comparisons. The embeddings separated three major immune branches—lymphocytes, myeloid cells, and platelets—and resolved over 10 biologically validated subtypes (CD4⁺ T, T reg, NK, classical and non-classical monocytes) with a macro-F1 of 0.92, delivering a high-resolution snapshot of circulating immune dynamics during respiratory infection.