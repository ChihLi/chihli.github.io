---
layout: archive
title: "Research"
permalink: /portfolio/
author_profile: true
---

{% include base_path %}

My research is rooted in the area of Computer Experiments/Uncertainty Quantification, but spans a range of applications from COVID-19 analysis to deep learning.


<img src='/images/researchroot.png' width="400" height="400" style="float:right">


Computer model simulations have become increasingly important for studying complex phenomena, such as climate change, response to natural crises, and the spread of pandemic diseases. Despite the popular use of computer simulations, they often encounter three challenges in practice:

* many computer simulations are prohibitively expensive, which require conducting an experiment by which a cheaper, accurate statistical emulator needs to be developed to approximate the computer simulations;
* computer models may be imperfect, so in order to make meaningful predictions, it is essential to calibrate a computer model by aligning the model's response with physical experimental data such that it can accurately reflect the real-world system;
* optimizing computer model outputs that are expensive to simulate can be almost impossible.

My research focus is to tackle these challenges by providing modern, efficient statistical approaches.

{% for post in site.portfolio %}
  {% include archive-single.html %}
{% endfor %}
