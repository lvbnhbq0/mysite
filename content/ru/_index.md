---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

design:
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      username: me-ru
      text: ''
      button:
        text: Скачать CV
        url: uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      background:
        gradient_mesh:
          enable: true
      name:
        size: md
      avatar:
        size: medium
        shape: circle
  - block: markdown
    content:
      title: '📚 Исследования и учёба'
      subtitle: ''
      text: |-
        Здесь кратко о том, чем занимаюсь: интересуюсь машинным обучением, анализом данных и прикладной математикой. В блоге — заметки по учёбе, лабораторным и инструментам.

        Если есть идеи для совместной работы или обсуждения — напишите, буду рада ответить.
    design:
      columns: '1'
  - block: collection
    id: news
    content:
      title: Последние новости
      subtitle: ''
      text: ''
      page_type: blog
      count: 10
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      offset: 0
      order: desc
    design:
      view: card
      spacing:
        padding: [0, 0, 0, 0]
  - block: cta-card
    demo: false
    content:
      title: 👉 Свой академический сайт на HugoBlox
      text: |-
        Этот сайт собран на **HugoBlox Kit** — открытом генераторе на Hugo, которым пользуются десятки тысяч исследователей и студентов.

        Можно собирать страницы из блоков без тяжёлой вёрстки: лендинги, курсы, портфолио и блоги.
      button:
        text: Шаблоны HugoBlox
        url: https://hugoblox.com/templates/
    design:
      card:
        css_class: 'bg-primary-300 dark:bg-primary-700'
        css_style: ''
---
