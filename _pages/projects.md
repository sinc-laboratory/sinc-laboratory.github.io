---
layout: single
title: "Projects"
permalink: /projects/
classes: wide2
---

{% assign projectsInOrder = site.projects | sort:"order" %}
{% for project in projectsInOrder %}
<h2  class="archive__subtitle">{{ project.title }}</h2>
<img src="{{ project.image_path | relative_url }}" class="project__image" alt="{{ project.image_description }}">
<p class="archive__item-excerpt" itemprop="description">
  {{ project.content }}
</p>
<div class="project__selected_publications">
<h3> Selected publications (<a href="{{ project.path | replace:'_projects','/publications' | replace:'.md','' }}">see all</a>)</h3>
<ul>
{% for publicationPermalink in project.selected_publications %}
  {% assign publication = site.publications | where:"permalink",publicationPermalink | first %}
  <li><a href="{{ publicationPermalink }}">{{ publication.title }} (<i>{{ publication.venue_short }}</i>)</a></li>
{% endfor %}
</ul>
</div>
{% endfor %}
