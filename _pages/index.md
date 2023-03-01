---
layout: page
title: Home
id: home
permalink: /
---

<strong>Notes:</strong>

<ul>
  {% assign recent_notes = site.notes%}
  {% for note in recent_notes%}
    <li>
      <a class="internal-link" href="{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
