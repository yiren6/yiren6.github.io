---
title: "VortexNet: A Graph Neural Network-Based Multi-Fidelity Surrogate Model for Field Predictions"
collection: talks
type: "Conference Talk"
permalink: /talks/2025-01-07-scitech-vortexnet
venue: "AIAA SciTech 2025 Forum"
date: 2025-01-07
location: "Orlando, FL, USA"
---

[Manuscript](https://arc.aiaa.org/doi/abs/10.2514/6.2025-0494) | [Slides](http://yiren6.github.io/files/Shen_Scitech_2025_VortexNet.pdf)

Aircraft design relies on accurate aerodynamic predictions. High-fidelity (HF) methods, such as computational fluid dynamics (CFD), provide accurate aerodynamic analyses but are computationally expensive for early-stage design. Conversely, low-fidelity (LF) methods, such as the vortex lattice method (VLM), offer cost-effective solutions but struggle to capture complex flow phenomena, limiting their predictive accuracy. This study introduces VortexNet, a graph neural network (GNN)-based surrogate model designed to bridge the fidelity gap between LF and HF aerodynamic predictions. VortexNet learns corrections to LF panel-wise local loading coefficient field data using data-driven insights from HF CFD simulations, enabling pressure coefficient field predictions across a range of delta wing geometries and free-stream conditions. The model demonstrates strong prediction accuracy and generalizability across configurations, effectively capturing nonlinear flow features under geometric variations. A hyper-parameter sensitivity study and a preliminary prediction mechanism explanation, leveraging the latent space ablation technique, are conducted to rationalize the model's predictive capabilities and provide guidance for future improvements in VortexNet-like surrogate modeling.
