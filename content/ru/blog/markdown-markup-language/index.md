---
title: 'Markdown — облегчённый язык разметки'
summary: Что такое Markdown, почему его любят для документации и статических сайтов и чем он проще «тяжёлых» форматов.
date: 2026-03-31

image:
  caption: 'Dustin Curtis (mark) — [Markdown-mark.svg](https://commons.wikimedia.org/wiki/File:Markdown-mark.svg) ([CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/deed.en), [Wikimedia Commons](https://commons.wikimedia.org/)); превью PNG с Commons. Оригинал: [markdown-mark](https://github.com/dcurtis/markdown-mark).'
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
  - me-ru

tags:
  - Markdown
  - Документация
  - Инструменты
---

**Markdown** — **облегчённый язык разметки**: пишете обычный текст с небольшим набором правил (заголовки `#`, курсив `*`, списки `-`, ссылки `[текст](url)` и т.д.), а рендерер превращает это в **HTML** или другие форматы. Формат задуман так, чтобы **было удобно читать исходник** и быстро набирать текст — в отличие от файлов текстовых процессоров, `.md` **удобно сравнивать в Git**, поэтому Markdown повсюду в **README**, **вики** и **генераторах статических сайтов** вроде Hugo.

По сравнению с **XML** или полным **HTML** в Markdown меньше шаблонного кода; по сравнению с **LaTeX** из коробки нет тонкой типографики для печати (хотя в многих пайплайнах можно встраивать формулы). **CommonMark** и диалекты вроде **GitHub Flavored Markdown** добавляют таблицы, чек-листы и блоки кода — технические тексты остаются приятными.

Для меня Markdown не абстракция: посты и страницы этого сайта — Markdown-файлы в репозитории, то есть как раз тот сценарий, ради которого формат и придумывался: **простой исходник, сильные инструменты, дружелюбный контроль версий**.
