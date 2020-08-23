---
layout: archive
permalink: /test/
title: "Test"
author_profile: true
header:
  image: "/images/workspace.jpg"
---

{% include base_path %}
{% include group-by-array collection=site.posts field="tags" %}

{% for tag in group_names %}
  <h2 id="{{ tag | slugify }}" class="archive__subtitle">{{ tag }}</h2>
  {% for post in posts %}
    {% include archive-single.html %}
{% endfor %}
