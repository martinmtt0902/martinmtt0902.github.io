---
title: "Diffusion Probabilistic Models under Gaussian Mixture Models"
collection: mini_projects
date: 2024-12-15
venue: "STAT6050 – Advanced Statistical Learning"
github: "https://github.com/martinmtt0902/Diffusion-Models"
project_type: "Individual project"
report_url: "https://github.com/martinmtt0902/Diffusion-Models/blob/main/report.pdf"
code_url: "https://github.com/martinmtt0902/Diffusion-Models/blob/main/code.R"
---

This project studies diffusion probabilistic models under Gaussian mixture models and compares several major samplers under the same target distribution. The work focuses on both theoretical understanding and practical performance across dimensions.

## Highlights
- Derived the exact score function for variance-preserving diffusion under a Gaussian mixture model.
- Implemented five samplers in R: DDPM, DDIM, DPM-Solver, DPM-Solver++, and UniPC.
- Compared sampling quality, computational efficiency, and robustness in a common experimental setting.
- Extended the analysis from low-dimensional examples to higher-dimensional cases.

## Methods
- Formulated the target model using Gaussian mixture distributions.
- Derived the analytical score function needed for diffusion-based sampling.
- Implemented each sampler in R and evaluated their behaviour under the same setup.

## Findings
- Different samplers showed clear tradeoffs between speed, stability, and output quality.
- The project helped clarify how solver choice affects performance in both simple and higher-dimensional settings.

## Resources
- [Report (PDF)](https://github.com/martinmtt0902/Diffusion-Models/blob/main/report.pdf)
- [R Code](https://github.com/martinmtt0902/Diffusion-Models/blob/main/code.R)
