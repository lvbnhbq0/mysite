---
title: Классификация токсичности текста
date: 2026-04-29
summary: Личный NLP-проект про токсичные или оскорбительные комментарии — гигиена датасета, базовые модели и калибровка до усложнения архитектуры.
tags:
  - NLP
  - Классификация
  - Python
links:
  - type: site
    url: https://github.com/lvbnhbq0

image:
  caption: 'Cepice — [A development of natural language processing tools.png](https://commons.wikimedia.org/wiki/File:A_development_of_natural_language_processing_tools.png) (схема NLP-инструментов; [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/deed.en), [Wikimedia Commons](https://commons.wikimedia.org/)); превью PNG с Commons, по центру на белом полотне.'
  filename: featured.png
---

Задача — **практическая поддержка модерации**: по короткому пользовательскому тексту выдать **оценку риска токсичности** с понятными ошибками — и ложные тревоги, и пропуски вредят сообществам одинаково сильно.

Фокус на **шуме разметки** (сарказм на грани, рекламируемый сленг, многоязычные фрагменты) и на **логистических / линейных baseline’ах** плюс компактный fine-tune трансформера только после стабильного контура оценки: стратифицированные сплиты, **баланс классов** и **калибровка** на валидации до прикосновения к тесту.

---
