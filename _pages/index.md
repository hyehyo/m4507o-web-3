---
layout: page
title: Home
id: home
permalink: /
---

<strong>recientes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<strong>música</strong>

[[tus señas]]

<strong>fotos</strong>

[[fotos sept. 2023]]

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
