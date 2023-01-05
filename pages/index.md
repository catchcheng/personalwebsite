---
layout: page
title: Catch Cheng
permalink: /
---

# Welcome to Catch Cheng's World

<!-- ![assets/img/docsy-jekyll.png](assets/img/docsy-jekyll.png) -->

{% for post in site.posts limit:10 %}

   <div class="post-preview">
   <h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
   <span class="post-date">{{ post.date | date: "%B %d, %Y" }}</span><br>
   {% if post.badges %}{% for badge in post.badges %}<span class="badge badge-{{ badge.type }}">{{ badge.tag }}</span>{% endfor %}{% endif %}
   <br><img src="{{ post.image }}" alt="drawing" width="30%"/><br>
   {{ post.content | split:'<!--more-->' | first }}
   {% if post.content contains '<!--more-->' %}
      <a href="{{ site.baseurl }}{{ post.url }}">read more</a>
   {% endif %}
   </div>
   <hr>
{% endfor %}

<!-- {{ site.repo }} -->
