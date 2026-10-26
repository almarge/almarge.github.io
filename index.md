---
layout: default
---
<h2>Articles</h2>
<ul>
  {% for post in site.posts %}
    <li style="margin-bottom: 2rem;">
      <span style="color: #666; font-size: 0.9rem;">{{ post.date | date: "%d/%m/%Y" }}</span>
      <h3 style="margin: 0;"><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    </li>
  {% endfor %}
</ul>
