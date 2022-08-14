---
layout: single
title: "Machine Listening for Environmental Sound Understanding"
permalink: /publications/machine-listening-for-environmental-sound-understanding
taxonomy: Environmental Machine Listening
classes: wide2
---

<section class="taxonomy__section">
{% for post in site.publications reversed %}
  {% if post.categories contains page.taxonomy %}
      <div class="entries-{{ page.entries_layout | default: 'list' }}">
          <p class="archive__item-excerpt" itemprop="description">
            <a href="{{ post.paperurl }}"><i class="fas fa-fw fa-file-pdf" aria-hidden="true"></i></a>
            <a href="{{ post.permalink }}">
            {{ post.citation }} </a>
          </p>
      </div>
  {% endif %}
{% endfor %}
</section>