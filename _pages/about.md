---
permalink: /
title: "About"
hide_title: true
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<div class="profile-page" markdown="1">

## Bio

Yiren Shen is a postdoctoral researcher working on AI-enabled design automation, physics-informed machine learning, and multi-fidelity optimization for sustainable aircraft and energy systems. His research sits at the intersection of aerospace design, surrogate modeling, and scientific machine learning. He develops graph neural networks and other data-driven methods to bridge low-fidelity and high-fidelity analyses, accelerate design-space exploration, and improve decision-making in conceptual aircraft design.

## Background

* Postdoctoral Researcher, NSF AI Institute in Dynamic Systems, University of Washington, 2026–present.
* Postdoctoral Researcher, Aerospace Design Lab, Stanford University, 2026.
* Research Fellow, GE Aerospace Research, Probabilistic Design and Material Informatics, 2025.
* Ph.D., Aeronautics and Astronautics, Stanford University, 2026. Advisor: Professor Juan J. Alonso.
* M.S., Aeronautics and Astronautics, Stanford University, 2019 (conferred 2024).
* B.S., Mechanical Engineering, Cornell University, 2017.

## Research

Three thrusts organize the work. **Multi-fidelity surrogates** learn corrections from fast aerodynamic models to high-fidelity flow fields. **Open data and benchmarks** supply the geometries, snapshots, and diagnostics those models are trained and compared on. **Design automation** puts the surrogates inside conceptual aircraft design, including stability-constrained wing optimization.

* **VortexNet.** A graph neural network that corrects low-fidelity panel loads into high-fidelity pressure fields for delta-wing aerodynamics.
* **Multi-fidelity conceptual design workflow.** Carries those field corrections into conceptual aircraft design, so early studies use CFD-level aerodynamic information.
* **Low-speed supersonic wing dataset.** An open multi-fidelity set of double-delta planforms, with vortex-lattice and RANS snapshots and scaling laws for how surrogate error changes with training-set size.
* **Stability-constrained wing design.** Graph-network-guided aerodynamic shape optimization of supersonic transport wings at low speed.
* **ShapeBench.** A benchmark and diagnostic suite for comparing aerodynamic shape optimization methods.

<p class="profile-links"><a href="https://dynamicsai.org/">NSF AI Institute in Dynamic Systems</a> <a href="https://adl.stanford.edu/">Stanford Aerospace Design Lab</a> <a href="https://huggingface.co/datasets/yirens/double-delta-aero">double-delta-aero dataset</a> <a href="https://github.com/yiren6/MF-VortexNet">MF-VortexNet github</a></p>

## Featured

<div class="feature-grid">
{% for post in site.posts %}
  {% if post.featured %}
  <a class="feature-tile" href="{{ post.url | relative_url }}">
    <div class="feature-tile__window">
      {% if post.figure %}
      <img class="feature-tile__figure" src="{{ post.figure | relative_url }}" alt="">
      {% endif %}
      <span>{{ post.kicker }}</span>
    </div>
    <div class="feature-tile__body">
      <h3 class="feature-tile__title">{{ post.title }}</h3>
      <p class="feature-tile__excerpt">{{ post.excerpt | strip_html | truncate: 150 }}</p>
    </div>
  </a>
  {% endif %}
{% endfor %}
</div>

## Publications

<ul class="pub-list">
{% assign pubs = site.publications | sort: "date" | reverse %}
{% for post in pubs limit: 6 %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span class="pub-meta">{{ post.venue }}, {{ post.date | date: "%Y" }}</span>
  </li>
{% endfor %}
</ul>

<p><a class="profile-more" href="{{ '/publications/' | relative_url }}">All publications</a></p>

</div>
