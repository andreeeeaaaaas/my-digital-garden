---
layout: page
title: Home
id: home
permalink: /
---
Hi, I'm Andreas 👋 <br>
— Welcome to my digital space.

I've tried holding my output in many iterations online over the years; this one feels the best.

<p style="padding: 2em 1em; background: #f5f7ff; border-radius: 8px;">
Click on <span style="font-weight: 600">[[Your first seed]]</span> to get started on your exploration.
</p>

<h4>[[Work]]</h4>
<h4>[[Studio]]</h4>
<h4>[[Writing]]</h4>


<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y · %m" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
