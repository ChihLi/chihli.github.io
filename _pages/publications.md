---
layout: archive
title: Publications
permalink: /publications/
author_profile: true
---

<style>
.page__title {
  display: none;
}
</style>

<p><span style="color: green;">color</span> indicates supervised student</p>

Preprints
======

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

<iframe 
  src="/barchart/publication-summary.html"
  width="100%"
  height="360"
  style="border:none; display:block;">
</iframe>

<p><span style="color: green;">color</span> indicates supervised student</p>

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
