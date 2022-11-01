---
layout: archive
title: Preprints
permalink: /publications/
author_profile: true
---

{% for post in site.submitted reversed %}
  {% include archive-single.html %}
{% endfor %}

{% include base_path %}

<br>

Refereed Papers
======

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
