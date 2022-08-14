---
layout: splash
permalink: /
redirect_from: 
  - /about/
  - /about.html
  - /home/
  - /home.html
header:
  overlay_color: "#800000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/red_voice_of_sinc.png
intro: 
  - excerpt: 'The Sound Interaction and Computing (SInC) Lab is headed by Prof. Mark Cartwright in the [Informatics Department of New Jersey Institute of Technology](https://informatics.njit.edu/). The lab pursues research at the intersection of human-computer interaction and machine learning with the aim of building tools to aid in the understanding and the creative expression of sound. To do so, the lab studies people’s needs and practices, researches new technology to meet those needs, and then studies how people use this new technology.'
---

The Sound Interaction and Computing (SInC) Lab is headed by Prof. Mark Cartwright in the [Informatics Department of New Jersey Institute of Technology](https://informatics.njit.edu/). The lab pursues research at the intersection of human-computer interaction and machine learning with the aim of building tools to aid in the understanding and the creative expression of sound. To do so, the lab studies people’s needs and practices, researches new technology to meet those needs, and then studies how people use this new technology.

Updates
-------
{% for post in site.posts limit:3  %}
  <a href="{{ post.url | relative_url }}" rel="permalink">{{ post.date | date: "%B %Y"}}</a> - {{ post.blurb }}
{% endfor %}
[&#8250; See all updates](/updates/)


Recent Publications
-------
{% assign recentPublications = site.publications | reverse %}
{% for post in recentPublications limit:5 %}
  <p class="archive__item-excerpt" itemprop="description">
    <a href="{{ post.paperurl }}"><i class="fas fa-fw fa-file-pdf" aria-hidden="true"></i></a>
    <a href="{{ post.permalink }}">
    {{ post.citation }} </a>
  </p>
{% endfor %}
[&#8250; See all publications](/publications)

