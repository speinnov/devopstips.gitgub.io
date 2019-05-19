---
layout: archive
title: "Devops for Talend Plateformeabout devops"
permalink: /devops/
author_profile: true
header:
  image: "/images/kadence_logo.png"
---

{% include nav_list %}


  {% for tag in group_names %}
    {% assign posts = group_items[forloop.index0] %}
    <h2 id="{{ tag  | slugify }}" class="archive__subtitle">{{ tag }}</h2>
    {% for post in posts % }
      {% include archive-single.html %}
    {% endfor%}
  {% endfor %}
