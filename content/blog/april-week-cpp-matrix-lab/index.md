---
title: 'This week — C++ vector & matrix classes lab (full marks)'
summary: I submitted the object-oriented linear-algebra lab on time, cleared the automated checks, and received the top grade after the oral review.
date: 2026-04-29

image:
  caption: 'GruenerBogen — [Transformation matrix diagram with colours.svg](https://commons.wikimedia.org/wiki/File:Transformation_matrix_diagram_with_colours.svg) (diagram of a linear map as a matrix; [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/deed.en), via [Wikimedia Commons](https://commons.wikimedia.org/)); PNG preview from Commons, centred on a white canvas.'
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
    name: "🏅"

authors:
  - me

tags:
  - C++
  - Linear algebra
  - Study
  - Weekly note
---

The **last week of April** was dominated by one heavy coursework item: a laboratory assignment on **classes for vectors and matrices in C++**, with operator overloads, basic numerical sanity checks, and a short **defence** in front of the instructor.

## What I built

I implemented a small **vector** type (fixed dimension known at compile time or passed at construction — per the spec), a **dense matrix** type, and the usual suspects: addition, scalar multiplication, **matrix–vector** and **matrix–matrix** products, transposition, and a few helpers for printing and comparing results to reference outputs. I also wired in simple **unit-style assertions** so regressions show up immediately when I change code late at night.

## Outcome

The checker scripts and the handwritten rubric items came back clean, and after walking through one **non-trivial multiply** example on the board, the instructor recorded **full marks**. Huge relief — and a good reminder that sweating the **interface design** early (names, const-correctness, clear invariants) saves debugging time later.

---
