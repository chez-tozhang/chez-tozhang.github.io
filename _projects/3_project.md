---
layout: page
title: Unsupervised Recovery of CLIP's Spatial Awareness
description: Enhancing CLIP's spatial understanding capabilities
img: assets/img/3.jpg
importance: 1
category: self-supervised
---

## Unsupervised Recovery of CLIP's Spatial Awareness

This research addresses a fundamental limitation in CLIP (Contrastive Language-Image Pre-training) models - their limited spatial understanding. Our approach enables CLIP to recover spatial awareness without requiring additional supervised training, significantly enhancing its capabilities for localization tasks.

### Research Motivation

While CLIP has demonstrated impressive zero-shot capabilities for image classification, its ability to perform spatial reasoning tasks like object localization or segmentation is limited. This limitation stems from the global pooling operations that discard spatial information in favor of semantic understanding.

### Our Approach

We developed an unsupervised method to recover spatial awareness in CLIP by:

- Designing a novel architectural modification that preserves spatial information
- Creating self-supervised tasks specifically targeting spatial understanding
- Implementing a multi-scale feature fusion mechanism to enhance localization precision
- Developing an adaptation technique that works with any pre-trained CLIP model

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="Method Overview" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="Heatmap Visualization" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/7.jpg" title="Quantitative Results" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: Overview of our approach for recovering spatial awareness in CLIP. Middle: Visualization of attention heatmaps before and after our method. Right: Quantitative improvements across various spatial reasoning tasks.
</div>

### Key Innovations

The core innovation of our work is the ability to enhance CLIP's spatial capabilities without requiring any labeled data. This makes our approach particularly valuable as it maintains CLIP's zero-shot capabilities while extending them to localization tasks.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/10.jpg" title="Qualitative Results" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Qualitative results demonstrating improved spatial understanding across various image types and query prompts.
</div>

### Applications and Results

Our spatially-aware CLIP model enables several new capabilities:

- **Zero-shot object localization**: Finding objects in images using only text descriptions
- **Text-guided segmentation**: Creating segmentation masks based on textual prompts
- **Compositional reasoning**: Understanding spatial relationships between multiple objects
- **Fine-grained visual grounding**: Localizing specific attributes or parts of objects

Our method achieves state-of-the-art performance on multiple benchmarks, improving over previous approaches by an average of 8.2% on localization tasks.

### Publications

This work has been accepted to ICLR 2025 and was led by Congpei Qiu. The paper and code will be made available upon publication.

### Acknowledgments

We thank our collaborators and the ICLR reviewers for their valuable feedback. This research was supported by computational resources from EPFL.
