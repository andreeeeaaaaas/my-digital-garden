---
layout: page-no-title
title: Home
id: home
permalink: /
---

<h2>Projects</h2>
<!-- <p>A collection of design, research, and work projects.</p> -->
<div class="bb">
  <flex class="align-baseline">
  <div style="min-width: 7em"><p>2023</p></div>
    <div>
      [[Co-designing Consent]]
      <p style="margin-top: 0.5rem; font-size: 0.875em" class="muted">Consent education is grounded in the human rights of a child, so why is it's delivery fettered with complication?</p>
    </div>
    </flex>
</div>

<div class="bb">
  <flex class="align-baseline">
  <div style="min-width: 7em"><p>2022</p></div>
    <div>
      [[Eli]]
      <p style="margin-top: 0.5rem; font-size: 0.875em" class="muted">An integrated physical and digital solution supporting students suffering from feelings of disconnectedness in remote learning environments.</p>
    </div>
    </flex>
</div>


<h2>Studio</h2>
<!-- <p>An amalgamation of music, photos, visuals and more.</p> -->

<h2>Latest notes</h2>
<ul style="list-style-type: none; padding-left: 0em;">
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y · %m" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>