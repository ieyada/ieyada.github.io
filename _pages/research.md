---
layout: archive
title: ""
permalink: /research/
author_profile: true
---
{% include base_path %}

## <center> <i> Working Papers </i> </center>
- - -

{% for post in site.workingpapers reversed %}
  {% include archive-single.html %}
{% endfor %}

## <center> <i> Publications </i> </center>
---

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}


{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}