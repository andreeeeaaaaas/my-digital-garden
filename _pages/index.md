---
layout: page
title: Home
id: home
permalink: /
---
<!-- <p style="padding: 2em 1em; background: #f5f7ff; border-radius: 8px;">
Want to know how to use this site? Click on <span style="font-weight: 600">[[your first seed]]</span> to get started on your exploration
</p> -->

<h2>Work</h2>
<p>A collection of design, research, and work projects.</p>

<h2>Studio</h2>
<p>An amalgamation of music, photos, visuals and more.</p>

<h2>Latest notes</h2>
<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y · %m" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>