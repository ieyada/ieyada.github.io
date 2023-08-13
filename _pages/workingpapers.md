---
layout: archive
title: "Working Papers"
permalink: /workingpapers/
author_profile: true
---

{% include base_path %}

{% for post in site.workingpapers reversed %}
  {% include archive-single.html %}
{% endfor %}


{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}
