---
layout: single
title: "Updates"
permalink: /updates/
classes: wide2
---

<div class="entries-{{ page.entries_layout | default: 'list' }}">
  {% for post in site.posts %}
    {% include archive-single.html type=entries_layout %}
  {% endfor %}
</div>