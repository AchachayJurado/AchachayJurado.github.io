---
title: "TryOffDiff: Virtual-Try-Off via High-Fidelity Garment Reconstruction using Diffusion Models"
collection: publications
permalink: /publication/2024-12-tryoffdiff
excerpt: 'diffusion models, virtual try-on, siglip, stable-diffusion, evaluation metrics'
date: 2024-11-27
venue: 'arXiv'
paperurl:
citation:
---

<b>Abstract---</b>
This paper introduces *Virtual Try-Off* (**VTOFF**), a novel task focused on generating standardized garment images from single photos of clothed individuals. Unlike traditional Virtual Try-On (VTON), which digitally dresses models, VTOFF aims to extract a canonical garment image, posing unique challenges in capturing garment shape, texture, and intricate patterns. This well-defined target makes VTOFF particularly effective for evaluating reconstruction fidelity in generative models. We present *TryOffDiff*, a model that adapts Stable Diffusion with SigLIP-based visual conditioning to ensure high fidelity and detail retention. Experiments on a modified VITON-HD dataset show that our approach outperforms baseline methods based on pose transfer and virtual try-on with fewer pre- and post-processing steps. Our analysis reveals that traditional image generation metrics inadequately assess reconstruction quality, prompting us to rely on DISTS for more accurate evaluation. Our results highlight the potential of VTOFF to enhance product imagery in e-commerce applications, advance generative model evaluation, and inspire future work on high-fidelity reconstruction.

[Project webpage](https://rizavelioglu.github.io/tryoffdiff/)

[//]: # (Demo)
<script type="module" src="https://gradio.s3-us-west-2.amazonaws.com/5.7.1/gradio.js"></script>
<gradio-app src="https://rizavelioglu-tryoffdiff.hf.space"></gradio-app>


Cited as:

```
@article{velioglu2024tryoffdiff,
    title     = {TryOffDiff: Virtual-Try-Off via High-Fidelity Garment Reconstruction using Diffusion Models},
    author    = {Velioglu, Riza and Bevandic, Petra and Chan, Robin and Hammer, Barbara},
    journal   = {arXiv},
    year      = {2024},
    note      = {\url{https://doi.org/nt3n}}
}
```
