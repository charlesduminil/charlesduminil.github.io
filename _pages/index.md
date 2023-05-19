---
layout: page
title: Home
id: home
permalink: /
---

# hello, welcome to the swamp 



<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  Take a look at <span style="font-weight: bold">[[start|I don't know what i'm doing but i'm doing it]]</span> to get started on your exploration.
</p>

This place is an attempt to document my very time-limited toughts and things i encounter on the fabulous world wide web. I explain more about the why [[About|here]].

<strong>Recently updated notes</strong>

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
