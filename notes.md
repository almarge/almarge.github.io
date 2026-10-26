---
layout: page
title: Notes
---
<div class="home">
  <ul class="post-list">
    {% for nota in site.notes %}
      <li>
        <h3><a class="post-link" style="color: #1a1a1a;" href="{{ nota.url | relative_url }}">{{ nota.title }}</a></h3>
      </li>
    {% endfor %}
  </ul>
</div>
