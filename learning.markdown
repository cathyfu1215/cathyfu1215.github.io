---
layout: page
title: "Learning"
permalink: /learning/
---

# Learning

Here are the classes I have taken:

<ul>
  {% for class in site.data.classes.classes %}
    <li>
      <h2>{{ class.title }}</h2>
      <p><strong>Institution:</strong> {{ class.institution }}</p>
      <p>{{ class.description }}</p>
      <p><strong>Mastery Level:</strong> {{ class.mastery_level }}</p>
      <ul>
        {% for link in class.links %}
          <li><a href="{{ link.url }}">{{ link.text }}</a></li>
        {% endfor %}
      </ul>
    </li>
  {% endfor %}
</ul>



