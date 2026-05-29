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

.keyword-btn {
  background: #F4F8F6;
  color: #18453B;
  border: 1px solid #DCE8E2;
  border-radius: 20px;
  padding: 6px 14px;
  font-size: 0.9em;
  font-weight: 500;
  cursor: pointer;
}

.keyword-btn:hover,
.keyword-btn.active {
  background: #18453B;
  color: white;
}

.filter-status {
  font-size: 0.9em;
  color: #666;
  margin-bottom: 15px;
}
</style>

Preprints
======

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

<iframe 
  src="/barchart/publication-summary.html"
  width="100%"
  height="360"
  style="border:none; display:block;">
</iframe>

<div class="keyword-container">
  <button class="keyword-btn active" data-filter="all">All</button>
  <button class="keyword-btn" data-filter="Computer Experiments">Computer Experiments</button>
  <button class="keyword-btn" data-filter="Uncertainty Quantification">Uncertainty Quantification</button>
  <button class="keyword-btn" data-filter="Multi-Fidelity Modeling">Multi-Fidelity Modeling</button>
  <button class="keyword-btn" data-filter="Gaussian Processes">Gaussian Processes</button>
  <button class="keyword-btn" data-filter="Deep Gaussian Processes">Deep Gaussian Processes</button>
  <button class="keyword-btn" data-filter="Surrogate Model">Surrogate Model</button>
  <button class="keyword-btn" data-filter="Computer Model Calibration">Computer Model Calibration</button>
  <button class="keyword-btn" data-filter="OOD Detection">OOD Detection </button>
  <button class="keyword-btn" data-filter="Inverse Problems">Inverse Problems</button>
</div>

<div class="filter-status" id="filter-status">
  Showing all publications.
</div>

<p><span style="color: green;">color</span> indicates supervised student</p>

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

<script>
document.addEventListener("DOMContentLoaded", function() {
  const buttons = document.querySelectorAll(".keyword-btn");
  const papers = document.querySelectorAll(".publication-item");
  const status = document.getElementById("filter-status");

  buttons.forEach(button => {
    button.addEventListener("click", function() {
      const keyword = this.dataset.filter;

      buttons.forEach(btn => btn.classList.remove("active"));
      this.classList.add("active");

      let count = 0;

      papers.forEach(paper => {
        const keywords = paper.dataset.keywords || "";

        if (keyword === "all" || keywords.includes(keyword)) {
          paper.style.display = "";
          count++;
        } else {
          paper.style.display = "none";
        }
      });

      if (keyword === "all") {
        status.textContent = "Showing all publications.";
      } else {
        status.textContent = "Showing publications tagged with: " + keyword + ".";
      }
    });
  });
});
</script>