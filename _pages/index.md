---
layout: page
title: Home
id: home
permalink: /
---

# Привет! Я fifkuks 🌱

Это мой цифровой сад, но здесь пока ничего нет (сэд фэйс). Вообще я обычно делаю заметки на бумаге и, скорее всего, редко сюда что-то буду постить

Мой <a class="external-link" href="https://t.me/fifkukstg" title="Telegram"></a>

## Содержание

- [[Радио]]

<strong>Недавно обновленные заметки</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%d-%m-%Y" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
