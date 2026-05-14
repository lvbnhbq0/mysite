---
title: Text toxicity classification
date: 2026-04-29
summary: A personal NLP project for detecting toxic or abusive comments — dataset hygiene, baselines, and calibration before chasing complex models.
tags:
  - NLP
  - Classification
  - Python
links:
  - type: site
    url: https://github.com/lvbnhbq0

image:
  caption: 'Cepice — [A development of natural language processing tools.png](https://commons.wikimedia.org/wiki/File:A_development_of_natural_language_processing_tools.png) (diagram of NLP tooling in research; [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/deed.en), via [Wikimedia Commons](https://commons.wikimedia.org/)); PNG preview from Commons, centred on a white canvas.'
  filename: featured.png
---

The aim here is **practical moderation support**: given short user-generated text, output a **toxicity risk score** with transparent errors — false alarms hurt communities just as much as misses.

I focused on **label noise** (borderline sarcasm, reclaimed language, multilingual snippets) and built **logistic / linear baselines** plus a compact transformer fine-tune only after the evaluation harness was stable: stratified splits, **class balance**, and **expected calibration** on validation before touching test.

---
