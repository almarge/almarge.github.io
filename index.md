---
layout: default
---
<div class="archive">
  <h2 class="section-label">Arxiu d'articles</h2>
  <ul class="archive-list">
    {% for post in site.posts %}
      <li class="archive-item">
        <a href="{{ post.url | relative_url }}" class="archive-link">
          <h3 class="archive-title">{{ post.title }}</h3>
          {% if post.subtitle %}
            <p class="archive-excerpt">{{ post.subtitle }}</p>
          {% else %}
            <p class="archive-excerpt">{{ post.content | strip_html | truncatewords: 18 }}</p>
          {% endif %}
          <time class="archive-date">{{ post.date | date: "%d · %m · %Y" }}</time>
        </a>
      </li>
    {% endfor %}
  </ul>
</div>
