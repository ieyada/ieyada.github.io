---
layout: archive
title: "Data"
permalink: /datasets/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.datasets reversed %}
  {% include archive-single.html %}
{% endfor %}
