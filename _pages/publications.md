---
layout: archive
title: 
permalink: /publications/
author_profile: true
---

Submitted
======

{% include base_path %}

{% for post in site.submitted reversed %}
  {% include archive-single.html %}
{% endfor %}


Publications
======

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
