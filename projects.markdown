---
layout: page
title: "Projects"
permalink: /projects/
---

Here are some of the projects I've worked on:

{% for project in site.projects %}
## <a href="{{ project.url }}">{{ project.title }}</a>
!Project Image

**Tags:** {{ project.tags | join: ', ' }}

<p>{{ project.description | truncatewords: 500 }}</p>

<a href="{{ project.url }}">Read more</a>

---

{% endfor %}

