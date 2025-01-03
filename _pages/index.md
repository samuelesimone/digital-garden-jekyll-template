---
layout: page
title: Home
id: home
permalink: /
---

# Hi, I'm Samuele Simone! 🌱
  <img style="border-radius: 50%; width:250px; height:250px" src="https://avatars.githubusercontent.com/u/33575158?v=4" alt="samuelesimone">

  <ul style="padding: 1em 1em; background: #f5f7ff; border-radius: 4px;">
    <li style="margin: 1em">PhD student in VRP and AI @ UNIMI</li>
    <li style="margin: 1em">If you want to know more about me <a class="internal-link" href="{{ site.baseurl }}/about">click here</a></li>
  </ul>


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
