---
layout: default
title: Notes
---
<div class="archive">
  <h2 class="section-label">Notes i apunts</h2>
  <ul class="archive-list">
    {% for nota in site.notes %}
      <li class="archive-item">
        <a href="{{ nota.url | relative_url }}" class="archive-link">
          <h3 class="archive-title">{{ nota.title }}</h3>
          <p class="archive-excerpt">{{ nota.content | strip_html | truncatewords: 22 }}</p>
        </a>
      </li>
    {% endfor %}
  </ul>
</div>
