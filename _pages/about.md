---
layout: single
title: "About"
permalink: /about/
---

## 저자 소개

<div class="authors">
  {% for author in site.authors %}
    <div class="author">
      {% include author-profile.html %}
    </div>
  {% endfor %}
</div>
