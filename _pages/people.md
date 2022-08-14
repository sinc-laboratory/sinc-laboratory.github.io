---
layout: single
title: "People"
permalink: /people/
classes: wide2
---

{% assign currentTeamMembers = site.team_members | where:"status", "Current" | sort:"order"%}
<section id="Current" class="people__section">
  <h2 class="archive__subtitle">Current</h2>
  <div class="grid__wrapper">
  {% for f in currentTeamMembers %}
    <div class="grid__item">
      <article class="archive__item" itemscope itemtype="https://schema.org/Person">
        <a href="{{ f.url }}">
          <img src="{{ f.image_path | relative_url }}" class="people__avatar">
          <h3 class="people__name">{{ f.name }}</h3>
          <h4 class="people__academic_title">{{ f.academic_title }}</h4>
        </a>
      </article>
    </div>
  {% endfor %}
  </div>
</section>


{% assign currentTeamMembers = site.team_members | where:"status", "Alumni" | sort:"order"%}
<section id="Alumni" class="people__section">
  <h2 class="archive__subtitle">Alumni</h2>
  <div class="grid__wrapper">
  {% for f in currentTeamMembers %}
    <div class="grid__item">
      <article class="archive__item" itemscope itemtype="https://schema.org/Person">
        {% if f.homepage_url %}
        <a href="{{ f.homepage_url }}">
        {% endif %}
          <img src="{{ f.image_path | relative_url }}" class="people__avatar">
          <h3 class="people__name">{{ f.name }}</h3>
          <h4 class="people__academic_title">{{ f.academic_title }}</h4>
        {% if f.homepage_url %}
        </a>
        {% endif %}
      </article>
    </div>
  {% endfor %}
  </div>
</section>


