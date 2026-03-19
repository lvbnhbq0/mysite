---
title: This week — Gaussian elimination for linear systems
summary: I implemented Gaussian elimination to solve systems of linear equations and successfully defended my work.
date: 2026-03-19

image:
  caption: 'Jirka Fiala — [Reduced row echelon form.svg](https://commons.wikimedia.org/wiki/File:Reduced_row_echelon_form.svg) ([CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/deed.en), via [Wikimedia Commons](https://commons.wikimedia.org/))'
  filename: featured.png

cover:
  image: featured.png
  position:
    x: 50
    y: 50
  overlay:
    enabled: true
    type: "gradient"
    opacity: 0.45
    gradient: "bottom"
  fade:
    enabled: true
    height: "80px"
  icon:
    name: "📐"

authors:
  - me

tags:
  - Linear algebra
  - Algorithms
  - Study
---

Over the past week I focused on **systems of linear algebraic equations (SLAEs)** and implemented **Gaussian elimination** in code — the classic way to turn a messy system into something you can actually solve step by step.

## How the algorithm works (in brief)

You start from the **augmented matrix** *[A | b]* that encodes **Ax = b** (unknown vector **x**).

1. **Forward elimination** — I go row by row and use **row operations** (swap rows, multiply a row by a non-zero scalar, add a multiple of one row to another) to create **zeros below the main diagonal**. The goal is **row echelon form**: each pivot sits to the right of the pivot above it, so the system becomes upper-triangular in shape.
2. If a pivot position ever has a zero where I need a non-zero, I **swap** with a lower row that has a non-zero in that column (partial pivoting helps with numerical stability).
3. **Back substitution** — once the system is upper-triangular, I solve from the **last equation upward**: the bottom row gives one variable directly, then I substitute upward until every component of **x** is known.

If the elimination reveals a row of zeros on the left but a non-zero on the right-hand side, the system is **inconsistent**. If I get all-zero rows on the left, I may have **free variables** and infinitely many solutions.

## Defence

I’m really glad to say I **successfully defended** this assignment: I walked through the method, showed how my implementation follows these steps, and answered the questions from the instructor. It was a good week — heavy on linear algebra, but it clicked once I saw elimination as “organising the matrix until back substitution is easy.”
