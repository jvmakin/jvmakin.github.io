---
layout: page
permalink: /projects/
title: projects
---

<ul class="post-list">
{% for poem in site.poetry reversed %}
    <li>
        <h2><a class="poem-title" href="{{ poem.url | prepend: site.baseurl }}">{{ poem.title }}</a></h2>
        {{ poem.description }}
        <p class="post-meta">{{ poem.date | date: '%B %-d, %Y' }}</p>

      </li>
{% endfor %}
</ul>
