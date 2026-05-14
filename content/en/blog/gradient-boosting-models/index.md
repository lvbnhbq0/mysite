---
title: 'Gradient boosting models — trees that learn from mistakes'
summary: How boosting builds an ensemble of weak learners, why shallow trees work, and where XGBoost-style systems fit in a modern ML stack.
date: 2026-05-13

image:
  caption: 'Hcho3wiki — [XGBoost logo.svg](https://commons.wikimedia.org/wiki/File:XGBoost_logo.svg) (logo of the XGBoost tree-boosting library; [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/deed.en), via [Wikimedia Commons](https://commons.wikimedia.org/)); PNG preview from Commons, centred on a white canvas. Project: [dmlc/xgboost](https://github.com/dmlc/xgboost).'
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
    name: "🌲"

authors:
  - me

tags:
  - Machine learning
  - Gradient boosting
  - Study
---

Around the **same mid-May stretch** as birthday prep, I revisited **gradient boosting** — the family of models that turned “decision stumps” into competition-winning tabular pipelines long before every leaderboard was a giant neural net.

## The core idea

Boosting starts with a **weak predictor** — usually a **shallow regression or classification tree** — and measures the **residual errors** it leaves behind. Each new tree is trained to predict those residuals (or a gradient-based proxy of the loss), and its predictions are **added** to the ensemble with a **learning rate** so updates stay stable. After enough rounds, the sum of tiny corrections behaves like a flexible nonlinear model with strong **out-of-sample** control if regularisation is tuned honestly.

## Practical ecosystems

Libraries such as **XGBoost**, **LightGBM**, and **CatBoost** wrap the same statistical idea with optimisations for **sparse data**, **missing values**, and **parallel tree construction**. In coursework I still reach for them first for **structured features**, and only swap to deep models when the signal genuinely lives in raw high-dimensional inputs.

---
