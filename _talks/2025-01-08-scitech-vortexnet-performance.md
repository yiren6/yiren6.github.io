---
title: "Performance Evaluation of a Graph Neural Network-Augmented Multi-Fidelity Workflow for Predicting Aerodynamic Coefficients on Delta Wings at Low Speed"
collection: talks
type: "Conference Talk"
permalink: /talks/2025-01-08-scitech-vortexnet-performance
venue: "AIAA SciTech 2025 Forum"
date: 2025-01-08
location: "Orlando, FL, USA"
---

[Manuscript](https://arc.aiaa.org/doi/abs/10.2514/6.2025-2360) | [Slides](http://yiren6.github.io/files/Shen_Scitech_2025_SCALOS.pdf)

Conceptual design of a stable and efficient supersonic transport (SST) aircraft during takeoff and landing, where higher angle-of-attack (AOA) induces complex aerodynamic phenomena such as vortex lift and flow separation, can be challenging. Existing analysis methods face a fidelity-cost trade-off: high-fidelity (HF) methods, such as computational fluid dynamics (CFD), offer prediction accuracy but are computationally expensive for solver-in-the-loop analyses, while low-fidelity (LF) methods, such as vortex lattice method (VLM), lack the ability to capture nonlinear flow physics. To address this gap, this paper proposes a multi-fidelity conceptual design analysis workflow that integrates a graph neural network (GNN)-based surrogate model into VLM to augment the analysis fidelity of LF tools. The surrogate model learns the discrepancies between LF and HF pressure fields, enabling accurate and efficient aerodynamic analyses on arbitrary quantities of interest. When evaluated on a dataset with various delta wing geometries, the proposed workflow achieves an approximately fivefold reduction in the normalized root mean square error (NRMSE) for the predicted lift, drag, and pitching moment coefficients compared to using VLM alone.
