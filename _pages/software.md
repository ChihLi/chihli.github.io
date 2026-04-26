---
layout: archive
title: "Software"
permalink: /software/
author_profile: true
redirect_from:
  - /software
---

{% include base_path %}

<style>

.page__title {
  display: none;
}

.software-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
  gap: 18px;
  margin-top: 15px;
}

.software-card {
  background: #ffffff;
  border: 1px solid rgba(0,0,0,0.08);
  border-radius: 10px;
  padding: 16px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.04);
}

.software-card a {
  font-weight: 700;
  color: #18453B;
  text-decoration: none;
}

.software-card p {
  font-size: 0.9em;
  margin: 8px 0 10px 0;
  line-height: 1.45;
}

.repro-list {
  margin-top: 12px;
}

.repro-item {
  margin-bottom: 14px;
  line-height: 1.5;
}

.repro-title a {
  font-weight: 600;
  color: #18453B;
  text-decoration: none;
}

.repro-meta {
  font-size: 0.85em;
  color: #666;
}
</style>

R Packages
======

The following packages implement methods developed in our research on Gaussian process modeling, computer experiments, calibration, and multi-fidelity emulation.

<div class="software-grid">

<div class="software-card">
<a href="https://cran.r-project.org/web/packages/MuFiMeshGP/index.html">MuFiMeshGP</a>
<p>Multi-fidelity emulator for computer experiments with tunable fidelity levels.</p>
<img src="https://cranlogs.r-pkg.org/badges/grand-total/MuFiMeshGP">
</div>

<div class="software-card">
<a href="https://cran.r-project.org/web/packages/DNAmf/index.html">DNAmf</a>
<p>Diffusion non-additive model with tunable precision.</p>
<img src="https://cranlogs.r-pkg.org/badges/grand-total/DNAmf">
</div>

<div class="software-card">
<a href="https://cran.r-project.org/web/packages/RNAmf/index.html">RNAmf</a>
<p>Recursive non-additive emulator for multi-fidelity data.</p>
<img src="https://cranlogs.r-pkg.org/badges/grand-total/RNAmf">
</div>

<div class="software-card">
<a href="https://github.com/ChihLi/mcGP">mcGP</a>
<p>Mesh-clustered Gaussian process emulator for PDE boundary value problems.</p>
</div>

<div class="software-card">
<a href="https://github.com/ChihLi/GPcluster">GPcluster</a>
<p>Clustered Gaussian process modeling for computer experiments.</p>
</div>

<div class="software-card">
<a href="https://github.com/ChihLi/HetCalibrate">HetCalibrate</a>
<p>Calibration parameter estimation for inexact computer models with heteroscedastic errors.</p>
</div>

<div class="software-card">
<a href="https://cran.r-project.org/web/packages/calibrateBinary/index.html">calibrateBinary</a>
<p>Calibration for computer experiments with binary responses.</p>
<img src="https://cranlogs.r-pkg.org/badges/grand-total/calibrateBinary">
</div>

<div class="software-card">
<a href="https://cran.r-project.org/web/packages/binaryGP/index.html">binaryGP</a>
<p>Gaussian process modeling for time-series binary responses.</p>
<img src="https://cranlogs.r-pkg.org/badges/grand-total/binaryGP">
</div>

<div class="software-card">
<a href="https://cran.r-project.org/web/packages/MRFA/index.html">MRFA</a>
<p>Multi-resolution functional ANOVA for large-scale nonlinear regression.</p>
<img src="https://cranlogs.r-pkg.org/badges/grand-total/MRFA">
</div>

</div>

<br>

Research Code & Reproducibility
======

Code repositories for reproducing results in our published work.

<div class="repro-list">

<div class="repro-item">
  <div class="repro-title">
    <a href="https://github.com/heojunoh/DNAmf-Reproducibility">
      Diffusion non-additive model for multi-fidelity simulations with tunable precision
    </a>
  </div>
  <div class="repro-meta">2025+ • GitHub repository</div>
</div>

<div class="repro-item">
  <div class="repro-title">
    <a href="https://github.com/YangChencyy/Uncertainty-Aware-Out-of-Distribution-Detection-with-Gaussian-Processes">
      Uncertainty-aware out-of-distribution detection with Gaussian processes
    </a>
  </div>
  <div class="repro-meta">2024+ • GitHub repository</div>
</div>

<div class="repro-item">
  <div class="repro-title">
    <a href="https://github.com/ChihLi/Bayes-Inverse-FIGP">
      Advancing inverse scattering with surrogate modeling and Bayesian inference for functional inputs
    </a>
  </div>
  <div class="repro-meta">2025 • SIAM/ASA Journal on Uncertainty Quantification</div>
</div>

<div class="repro-item">
  <div class="repro-title">
    <a href="https://github.com/heojunoh/RNAmf-Reproducibility">
      Active learning for a recursive non-additive emulator for multi-fidelity computer experiments
    </a>
  </div>
  <div class="repro-meta">2025 • Technometrics</div>
</div>

<div class="repro-item">
  <div class="repro-title">
    <a href="https://github.com/sagalin14/ctGP">
      Category tree Gaussian process for computer experiments with many-category qualitative factors
    </a>
  </div>
  <div class="repro-meta">2024 • Journal of Quality Technology</div>
</div>

<div class="repro-item">
  <div class="repro-title">
    <a href="https://github.com/ChihLi/mcGP-Reproducibility">
      Mesh-clustered Gaussian process emulator for PDE boundary value problems
    </a>
  </div>
  <div class="repro-meta">2024 • Technometrics</div>
</div>

<div class="repro-item">
  <div class="repro-title">
    <a href="https://github.com/ChihLi/StackingDesign-Reproducibility">
      Stacking designs: designing multifidelity computer experiments with target predictive accuracy
    </a>
  </div>
  <div class="repro-meta">2024 • SIAM/ASA Journal on Uncertainty Quantification</div>
</div>

<div class="repro-item">
  <div class="repro-title">
    <a href="https://github.com/ChihLi/Epidemic-Models-Calibration">
      Efficient calibration for imperfect epidemic models with applications to COVID-19
    </a>
  </div>
  <div class="repro-meta">2024 • Journal of the Royal Statistical Society: Series C</div>
</div>

<div class="repro-item">
  <div class="repro-title">
    <a href="https://github.com/ChihLi/functional-input-GP">
      Functional-input Gaussian processes with applications to inverse scattering problems
    </a>
  </div>
  <div class="repro-meta">2024 • Statistica Sinica</div>
</div>

<div class="repro-item">
  <div class="repro-title">
    <a href="https://github.com/ChihLi/HetCalibrate-Reproducibility">
      Calibration of inexact computer models with heteroscedastic errors
    </a>
  </div>
  <div class="repro-meta">2022 • SIAM/ASA Journal on Uncertainty Quantification</div>
</div>

<div class="repro-item">
  <div class="repro-title">
    <a href="https://github.com/ChihLi/Understanding-Impact-of-weather-and-intervention-on-COVID-19-AoAs">
      Estimating functional parameters for understanding the impact of weather and interventions on COVID-19
    </a>
  </div>
  <div class="repro-meta">2022 • Annals of Applied Statistics</div>
</div>

<div class="repro-item">
  <div class="repro-title">
    <a href="https://github.com/jasa-acs/An-efficient-surrogate-model-for-emulation-and-physics-extraction-of-large-eddy-simulations">
      An efficient surrogate model for emulation and physics extraction of large eddy simulations
    </a>
  </div>
  <div class="repro-meta">2018 • Journal of the American Statistical Association</div>
</div>

</div>