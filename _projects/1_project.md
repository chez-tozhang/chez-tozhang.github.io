---
layout: page
title: SINDER
description: Repairing the Singular Defects of DINOv2
img: assets/img/1.jpg
importance: 1
category: computer-vision
---

## SINDER: Repairing the Singular Defects of DINOv2

This project presents a novel approach to examining and repairing defects in vision foundation models, particularly focusing on DINOv2. Our method achieves significant efficiency improvements—saving over 3,000 GPU hours compared to existing methods.

### Key Innovations

- Identified and characterized singular defects in DINOv2's representation space
- Developed a lightweight repair method that preserves beneficial properties while addressing defects
- Created efficient analysis tools for understanding vision foundation model behavior
- Demonstrated improved performance across various downstream tasks

### Technical Details

Our approach begins by analyzing the eigenvalue spectrum of the representation space, identifying problematic "singular" dimensions that cause performance degradation. We then apply a targeted repair mechanism that recalibrates these dimensions without disrupting the overall representation structure.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="SINDER Overview" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="Performance Improvement" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="Singular Value Distribution" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: Overview of the SINDER approach. Middle: Performance improvements across benchmark tasks. Right: Analysis of singular value distribution before and after repair.
</div>

### Results and Impact

Our method demonstrates consistent improvements across a range of computer vision tasks:

- Object detection: +2.3% mAP on COCO
- Semantic segmentation: +1.8% mIoU on ADE20K
- Visual question answering: +1.5% accuracy on VQAv2

Importantly, these gains come with minimal computational overhead, making SINDER practical for real-world applications.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="Qualitative Results" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="Attention Maps" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Qualitative results showing improved visual understanding and attention maps after applying SINDER.
</div>

### Publications and Code

This research has been accepted as an **oral presentation** at ECCV 2024.

The code for SINDER is available on GitHub: [SINDER Repository](https://github.com/IVRL/SINDER)

### Acknowledgments

This work was led by Haoqi Wang as her first project at EPFL. We thank our collaborators and acknowledge the computational resources provided by EPFL.

