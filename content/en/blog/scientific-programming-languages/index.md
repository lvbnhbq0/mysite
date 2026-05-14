---
title: 'Languages for scientific programming — a quick map'
summary: From Fortran and MATLAB to Julia, R, and Python stacks — how different ecosystems trade speed, libraries, and ergonomics for research code.
date: 2026-04-30

image:
  caption: 'Official [Julia Programming Language Logo](https://commons.wikimedia.org/wiki/File:Julia_Programming_Language_Logo.svg) ([MIT licence](https://opensource.org/licenses/MIT), Julia project / Wikimedia Commons); PNG preview from Commons, centred on a white canvas. Used here as a representative of modern scientific computing stacks.'
  filename: featured.png

cover:
  image: featured.png
  position:
    x: 50
    y: 50
  overlay:
    enabled: true
    type: "gradient"
    opacity: 0.32
    gradient: "bottom"
  fade:
    enabled: true
    height: "80px"
  icon:
    name: "🔭"

authors:
  - me

tags:
  - Scientific computing
  - Programming languages
  - Study
---

Around the **end of April**, while the C++ lab was wrapping up, I wrote a short comparison note for myself on **languages used in scientific programming** — not “which is best,” but **which tool fits which bottleneck**.

## The usual suspects

**Fortran** and **C/C++** still underpin a lot of performance-critical simulation and legacy libraries: predictable memory, mature compilers, and decades of numerical practice.

**MATLAB** (and similar proprietary environments) remain strong where licences exist and **matrix workflows** are interactive: fast experimentation, rich toolboxes, and polished visualisation — at the cost of portability and long-term reproducibility outside the ecosystem.

**R** dominates many **statistics-heavy** pipelines; **Python** with **NumPy / SciPy / pandas** is the default glue language for data, deep learning wrappers, and automation.

**Julia** targets the “two-language problem” by aiming for **interactive high-level code** that can still approach native speed for well-structured numerical kernels — with a growing ecosystem in optimisation, differential equations, and scientific ML.

## Takeaway

For coursework I mostly stay in **C++** (structures + performance discipline) and **Python** (experimentation). Knowing **where each language wins** helps me pick a sane default before optimising the wrong layer.

---
