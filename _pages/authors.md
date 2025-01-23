---
layout: single
title: "Authors"
permalink: /authors/
---

## 저자 소개

<div class="authors">
  {% for author_key in site.data.authors | keys %}
    {% assign author = site.data.authors[author_key] %}
    <div class="author">
      <img src="{{ author.avatar }}" alt="{{ author.name }}" class="author-avatar" />
      <h3>{{ author.name }}</h3>
      <p>{{ author.bio }}</p>
      <p class="social-links">
        {% for link in author.links %}
          <a href="{{ link.url }}" target="_blank">
            <i class="{{ link.icon }}"></i> {{ link.label }}
          </a>
        {% endfor %}
      </p>
    </div>
  {% endfor %}
</div>
