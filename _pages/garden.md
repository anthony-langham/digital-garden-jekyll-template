---
layout: page
title: garden
permalink: /garden
---

# 🌱 garden

This is my digital garden, my small piece of the internet to write and think freely, without having to consider how to write a perfect blog post.

Some of the writing is bad. Some is okay. Some parts are missing. It's a work in progress, much like a real garden. Feel free to take a look around!
<br>
<br>
<strong>Recent updates:</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>
<br>
<br>
<strong>Graph / Map:</strong>
{% include notes_graph.html %}

<!-- <style>
  .wrapper {
    max-width: 46em;
  }
</style> -->
