---
layout: archive
permalink: /portfolio/
title: "Data Science Portfolio"
author_profile: true
header:
  image: "/images/workspace.jpg"
---

{% if page.header.overlay_color or page.header.overlay_image or page.header.image %}
  {% include page__hero.html %}
{% elsif page.header.video.id and page.header.video.provider %}
  {% include page__hero_video.html %}
{% endif %}

{% if page.url != "/" and site.breadcrumbs %}
  {% unless paginator %}
    {% include breadcrumbs.html %}
  {% endunless %}
{% endif %}
