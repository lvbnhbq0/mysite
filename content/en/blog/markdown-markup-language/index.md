---
title: 'Markdown — a lightweight markup language'
summary: What Markdown is, why it is popular for docs and static sites, and how it differs from heavier formats.
date: 2026-03-31

image:
  caption: 'Dustin Curtis (mark) — [Markdown-mark.svg](https://commons.wikimedia.org/wiki/File:Markdown-mark.svg) ([CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/deed.en), via [Wikimedia Commons](https://commons.wikimedia.org/)); PNG preview from Commons. Original: [markdown-mark](https://github.com/dcurtis/markdown-mark).'
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
    name: "📝"

authors:
  - me

tags:
  - Markdown
  - Documentation
  - Tools
---

**Markdown** is a **lightweight markup language**: you write plain text with a small set of conventions (headings with `#`, emphasis with `*`, lists with `-`, links with `[text](url)`, and so on), and a renderer turns it into **HTML** or other formats. It was designed to be **readable as-is** and fast to type — unlike word-processor files, a `.md` file diffs cleanly in Git, which is why it dominates **READMEs**, **wikis**, and **static site generators** like Hugo.

Compared with **XML** or full **HTML**, Markdown hides most boilerplate; compared with **LaTeX**, it does not aim at fine-grained print typography out of the box (though you can embed LaTeX math in many Markdown pipelines). **CommonMark** and flavours such as **GitHub Flavoured Markdown** add tables, task lists, and fenced code blocks so technical writing stays pleasant.

For me, Markdown is not an abstract topic: this site’s posts and pages are Markdown files in a repository, and that is exactly the workflow lightweight markup is meant to support — **simple source, strong tooling, happy version control**.
