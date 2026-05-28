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

.keyword-container {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin: 15px 0 25px 0;
}

.keyword {
  background: #F4F8F6;
  color: #18453B;
  border: 1px solid #DCE8E2;
  border-radius: 20px;
  padding: 6px 14px;
  font-size: 0.9em;
  font-weight: 500;
}

.keyword:hover {
  background: #18453B;
  color: white;
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

<div class="keyword-container">
  <span class="keyword">Computer Experiments</span>
  <span class="keyword">Uncertainty Quantification</span>
  <span class="keyword">Multi-Fidelity Modeling</span>
  <span class="keyword">Gaussian Processes</span>
  <span class="keyword">Bayesian Optimization</span>
  <span class="keyword">Deep Gaussian Processes</span>
  <span class="keyword">Digital Twins</span>
  <span class="keyword">Computer Model Calibration</span>
  <span class="keyword">Inverse Problems</span>
</div>

<p><span style="color: green;">color</span> indicates supervised student</p>

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
