---
layout: page
title: Projects
permalink: /docs/
---

# Projects

Welcome to the Catch's projects page! Here you can quickly jump to a particular category of my projects.

<div class="section-index">
    <hr class="panel-line">
    {% for post in site.docs  %}        
    <div class="entry">
    <h5><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h5>
    <!-- <p>{{ post.tag }}</p> how to add badges for projects -->
    <p>{{ post.description }}</p>
    </div>{% endfor %}
    <!-- <h>test</h>here decides the "Document page", which is ordered by letter -->
</div>
