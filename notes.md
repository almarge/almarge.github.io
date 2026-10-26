---
layout: default
---
<h2>Notes</h2>
<ul>
  {% for nota in site.notes %}
    <li style="margin-bottom: 1.5rem;">
      <h3 style="margin: 0;"><a href="{{ nota.url | relative_url }}">{{ nota.title }}</a></h3>
    </li>
  {% endfor %}
</ul>
