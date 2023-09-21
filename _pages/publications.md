---
layout: archive
title: Preprints
permalink: /publications/
author_profile: true
---

<p><span style="color: green;">color</span> indicates supervised student</p>

{% for post in site.submitted reversed %}
  {% include archive-single.html %}
{% endfor %}

{% include base_path %}

<br>

Publications
======

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

<iframe src="/barchart/publication-summary.html" height="300" width="850" style="border:none;"></iframe>

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
