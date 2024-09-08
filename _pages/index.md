---
layout: page
title: Home
id: home
permalink: /
---

# Welcome! 🌱

## Character Creation
[[01. Character Definitions]]
[[02. Crew Composition]]
[[03. Psionics]]
[[04. Crew Equipment]]
[[05. Ship Details & Loans]]






<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
