---
layout: page
title: wiki
permalink: /wiki
---

# Welcome to my Wiki

This is my personal digital garden. A wild garden, loosely tended. There's drafts, ideas, partials, fragments and ideas.

{% include notes_graph.html %}

<strong>Recently updated</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
