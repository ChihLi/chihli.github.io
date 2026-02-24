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

### Multi-Fidelity or Single-Fidelity?
 
In many scientific applications, researchers combine expensive high-accuracy simulations 
with cheaper low-accuracy ones. But is multi-fidelity modeling always better than 
using a single high-fidelity simulator?


In [this work](https://epubs.siam.org/doi/full/10.1137/22M1532007), we provide a theoretical understanding of 
when multi-fidelity emulation truly improves prediction accuracy — and when it does not. 
Our results reveal that blindly adding low-fidelity data can sometimes hurt performance. 
This work provides practical guidance for designing computer experiments efficiently.



### Beyond Linear Relationships in Multi-Fidelity Modeling

Traditional multi-fidelity models assume a simple linear relationship between 
low- and high-fidelity simulations. But real-world systems are rarely that simple.


In [this work](https://doi.org/10.1080/00401706.2024.2320211), we introduce the 
<strong>RNA (Recursive Non-Additive) model</strong>, which allows flexible nonlinear 
dependence across fidelities. This significantly improves predictive accuracy in 
complex engineering and scientific applications.


An open-source implementation is available in our 
[R package](https://cran.r-project.org/web/packages/RNAmf/index.html).


Grants
======
* [NSF DMS 2338018](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2338018): 2024-2029 (PI, $423,591) *CAREER: Single-Fidelity vs. Multi-Fidelity Computer Experiments: Unveiling the Effectiveness of Multi-Fidelity Emulation*
* [NSF DMS 2113407](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2113407&HistoricalAwards=false): 2021-2024 (PI, $142,009) *Collaborative Research: Efficient Bayesian Global Optimization with Applications to Deep Learning and Computer Experiments*

<img src='/images/MSUNSF.png' width="240" height="120" style="float:left">


