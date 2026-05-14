---
title: 'This week — transformers, labs, and site updates'
summary: A short recap of coursework, self-study on the Transformer architecture, and polishing this portfolio.
date: 2026-03-30

image:
  caption: 'dvgodoy — [Transformer, full architecture.png](https://commons.wikimedia.org/wiki/File:Transformer,_full_architecture.png) ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.en), via [Wikimedia Commons](https://commons.wikimedia.org/)); PNG preview from Commons. Source graphics: [dl-visuals](https://github.com/dvgodoy/dl-visuals).'
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
    name: "🧠"

authors:
  - me

tags:
  - Study
  - Deep learning
  - Weekly note
---

The last week of **March** was a mix of **regular university classes**, **small lab deadlines**, and **reading beyond the curriculum** so the ideas from lectures actually stick.

## Transformer architecture (self-study)

I spent focused time studying the **Transformer** architecture — the model family behind many modern language and vision systems. In a few words: instead of recurrence, a Transformer maps an entire sequence in parallel using **self-attention**, where each position learns to **attend** to other positions and build contextual representations. **Multi-head attention** runs several attention mechanisms in parallel; **positional encodings** tell the model about order; and **feed-forward blocks** refine each position. The encoder–decoder design (as in the original “Attention Is All You Need” paper) stacks these layers so the model can translate or generate structured outputs. It finally “clicked” when I traced how **queries, keys, and values** combine into one attention map.

## Everything else

I also tidied up **notes for linear algebra**, rehearsed an upcoming quiz, and updated this **HugoBlox** site with clearer résumé sections so skills, experience, and accomplishments stay in one place. Looking forward to April being a bit calmer — but the transformer rabbit hole was worth it.
