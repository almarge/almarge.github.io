---
layout: default
title: Notes
---
<div class="home">
  <h2 class="post-list-heading">Notes</h2>
  <ul class="post-list">
    {% for nota in site.notes %}
      <li>
        <h3><a class="post-link" style="color: #1a1a1a;" href="{{ nota.url | relative_url }}">{{ nota.title }}</a></h3>
      </li>
    {% endfor %}
  </ul>
</div>
