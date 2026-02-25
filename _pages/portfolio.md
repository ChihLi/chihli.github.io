---
layout: archive
title: "Research"
permalink: /portfolio/
author_profile: true
---

{% include base_path %}

My research is rooted in the area of Computer Experiments/Uncertainty Quantification/Digital Twins, but spans a range of applications from COVID-19 analysis to deep learning.


<img src='/images/researchroot.png' width="400" height="400" style="float:right">


Computer model simulations have become increasingly important for studying complex phenomena, such as climate change, response to natural crises, and the spread of pandemic diseases. Despite the popular use of computer simulations, they often encounter three challenges in practice:

* many computer simulations are prohibitively expensive, which require conducting an experiment by which a cheaper, accurate statistical emulator needs to be developed to approximate the computer simulations;
* computer models may be imperfect, so in order to make meaningful predictions, it is essential to calibrate a computer model by aligning the model's response with physical experimental data such that it can accurately reflect the real-world system;
* optimizing computer model outputs that are expensive to simulate can be almost impossible.

My research focus is to tackle these challenges by providing modern, efficient statistical approaches.



Highlighted Research Contributions
======

{% capture mf %}
**Multi-Fidelity or Single-Fidelity?**  
In many scientific applications, researchers combine expensive high-accuracy simulations with cheaper low-accuracy ones. But is multi-fidelity modeling always better than using a single high-fidelity simulator?

In [this work](https://epubs.siam.org/doi/full/10.1137/22M1532007) (Sung et al., 2024), we provide a theoretical understanding of when multi-fidelity emulation improves prediction accuracy — and when it does not. We show that blindly adding low-fidelity data can sometimes hurt performance, and we give guidance for designing computer experiments efficiently.

<span style="font-size: 0.82em; color: #6b6b6b;">
Sung, C.-L., Ji, Y., Mak, S., Wang, W., & Tang, T. (2024). *SIAM/ASA J. Uncertainty Quantification*, 12(1), 157–181.
</span>
{% endcapture %}
<div class="notice--primary">{{ mf | markdownify }}</div>

{% capture rna %}
**Beyond Linear Relationships in Multi-Fidelity Modeling**  
Traditional multi-fidelity models assume a simple linear relationship between low- and high-fidelity simulations. But real-world systems are rarely that simple.

In [this work](https://doi.org/10.1080/00401706.2024.2320211) (Heo and Sung, 2025), we introduce the **RNA (Recursive Non-Additive) model**, allowing flexible nonlinear dependence across fidelities and improving predictive accuracy in complex applications.

Open-source implementation: [RNAmf (CRAN)](https://cran.r-project.org/web/packages/RNAmf/index.html).

<span style="font-size: 0.82em; color: #6b6b6b;">
Heo, J., and Sung, C.-L. (2025). *Technometrics*, 67(1), 58-72.
</span>
{% endcapture %}
<div class="notice--info">{{ rna | markdownify }}</div>

{% capture rna %}
**Regression with Functional Inputs: When the Input is a Curve**

In many scientific problems, inputs are not just numbers — they can be entire functions. 
For example, instead of a scalar parameter, the input might be a curve such as 
$\sin(x)$, $\cos(x)$, or a spatial profile describing material properties.

In [this work](https://www3.stat.sinica.edu.tw/sstest/j34n4/j34n404/j34n404.html) (Sung et al., 2024), we develop a new class of Gaussian process models 
that can handle **functional inputs** directly. We introduce kernel functions designed 
for inputs that are curves or functions, rather than finite-dimensional vectors.

Open-source implementation: [Reproducibility (GitHub)](https://github.com/ChihLi/functional-input-GP).

<span style="font-size: 0.82em; color: #6b6b6b;">
Sung, C.-L., Wang, W., Cakoni, F., Harris, I., & Hung, Y. (2024). *Statistica Sinica*, 34(4), 1883-1902.
</span>
{% endcapture %}
<div class="notice--warning">{{ rna | markdownify }}</div>


Grants
======
* [NSF DMS 2338018](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2338018): 2024-2029 (PI, $423,591) *CAREER: Single-Fidelity vs. Multi-Fidelity Computer Experiments: Unveiling the Effectiveness of Multi-Fidelity Emulation*
* [NSF DMS 2113407](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2113407&HistoricalAwards=false): 2021-2024 (PI, $142,009) *Collaborative Research: Efficient Bayesian Global Optimization with Applications to Deep Learning and Computer Experiments*

<img src='/images/MSUNSF.png' width="240" height="120" style="float:left">


