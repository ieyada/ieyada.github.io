---
layout: archive
title: "Papers"
permalink: /papers/
author_profile: true
---
{% include base_path %}

* <center> Working Papers </center>*
- - -

{% for post in site.workingpapers reversed %}
  {% include archive-single.html %}
{% endfor %}

* <center> Publications </center>*
---

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}


{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}