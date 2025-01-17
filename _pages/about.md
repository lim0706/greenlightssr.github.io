---
layout: single
title: "About"
permalink: /about/
---

## 저자 소개

<div class="authors">
  {% for author_key, author in site.data.authors %}
    <div class="author">
      <img src="{{ author.avatar }}" alt="{{ author.name }}" class="author-avatar" />
      <h3>{{ author.name }}</h3>
      <p>{{ author.bio }}</p>
      <p class="social-links">
        {% if author.website %}
          <a href="{{ author.website }}" target="_blank">Website</a>
        {% endif %}
        {% if author.linkedin %}
          <a href="{{ author.linkedin }}" target="_blank">LinkedIn</a>
        {% endif %}
        {% if author.github %}
          <a href="{{ author.github }}" target="_blank">GitHub</a>
        {% endif %}
      </p>
    </div>
  {% endfor %}
</div>
