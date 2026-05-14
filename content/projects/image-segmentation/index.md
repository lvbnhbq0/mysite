---
title: Image segmentation for objects
date: 2026-04-29
summary: A personal project exploring pixel-level masks on natural images — classical colour clustering versus lightweight trainable pipelines.
tags:
  - Computer vision
  - Segmentation
  - Python
links:
  - type: site
    url: https://github.com/lvbnhbq0

image:
  caption: 'Zeonzir — [Sample segmentation HMRF-EM.png](https://commons.wikimedia.org/wiki/File:Sample_segmentation_HMRF-EM.png) (HMRF–EM colour segmentation into three regions; [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/deed.en), via [Wikimedia Commons](https://commons.wikimedia.org/)); original illustration; centred on a white canvas for this site.'
  filename: featured.png
---

This project started as a sandbox for **object-level masks**: given an RGB photograph, produce a label map that separates foreground instances or coherent regions well enough for downstream metrics.

I compared a **classical colour-clustering baseline** (fast to iterate, brittle under lighting) with a **small fully convolutional head** trained on a tiny hand-labelled subset. The goal was not SOTA benchmarks, but a clean repo layout, reproducible dataloading, and honest **IoU / boundary-F** reporting on held-out frames.

---
