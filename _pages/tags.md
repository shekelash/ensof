---
layout: page
title: Tags
permalink: /tags
---

# Tags

<ul class="tags">
{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for note in tag[1] %}
      <li><a href="{{ note.url }}">{{ note.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
</ul>