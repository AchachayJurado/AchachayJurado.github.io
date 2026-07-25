---
title: "FashionFail: Addressing Failure Cases in Fashion Object Detection and Segmentation"
collection: publications
permalink: /publication/2024-04-fashionfail
excerpt: 'object detection, instance segmentation, fashion parsing, dataset, robustness, annotation tool'
date: 2024-04-12
venue: 'International Joint Conference on Neural Networks (IJCNN)'
paperurl:
citation:
---

<b>Abstract---</b>
In the realm of fashion object detection and segmentation for online shopping images, existing state-of-the-art fashion parsing models encounter limitations, particularly when exposed to non-model-worn apparel and close-up shots. To address these failures, we introduce FashionFail; a new fashion dataset with e-commerce images for object detection and segmentation. The dataset is efficiently curated using our novel annotation tool that leverages recent foundation models.
The primary objective of FashionFail is to serve as a test bed for evaluating the robustness of models. Our analysis reveals the shortcomings of leading models, such as Attribute-Mask R-CNN and Fashionformer. Additionally, we propose a baseline approach using naive data augmentation to mitigate common failure cases and improve model robustness. Through this work, we aim to inspire and support further research in fashion item detection and segmentation for industrial applications.

[Project webpage](https://rizavelioglu.github.io/fashionfail/)

[//]: # (Demo)
<script type="module" src="https://gradio.s3-us-west-2.amazonaws.com/4.26.0/gradio.js"></script>
<gradio-app src="https://rizavelioglu-fashionfail.hf.space"></gradio-app>




Cited as:

```
@inproceedings{velioglu2024fashionfail,
  author    = {Velioglu, Riza and Chan, Robin and Hammer, Barbara},
  title     = {FashionFail: Addressing Failure Cases in Fashion Object Detection and Segmentation},
  booktitle = {IJCNN},
  year      = {2024},
  doi       = {https://doi.org/ng59},
  eprint    = {2404.08582}
}
```
