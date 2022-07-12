---
layout: page
title: project 6
description: The Retrieval of the Beautiful - Self-supervised Salient Object Detection for Beauty Product Retrieval (ACMMM)
img: assets/img/9.jpg
importance: 6
category: work
---

Beauty product retrieval is a challenging task due to the severe
image variation issue in real-world scenes.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Beau_task.png" title="Beau_task" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
     Examples of beauty product retrieval problem. The query images are always vary from the database images, such as viewpoint variation, deformation, illumination conditions and background clutter.
</div>

In this work, to mitigate the data variation problem, we contribute a background-agnostic feature extractor, which is trained by a self-supervised salient object detection method.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Beau_framework.png" title="Beau_framework" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The illustration of foreground augmentation stage.
</div>

In particular, we first propose a foreground augmentation technique to acquire the augmentation image with its foreground mask. Next, a feature extractor with an attention pooling layer is proposed to learn background-agnostic representations by performing the salient object detection in a self-supervised manner. Finally, we ensemble the background-agnostic features of multiple models to perform the beauty product retrieval. 

<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/Beau_results2.png" title="Beau_results2" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/Beau_results.png" title="Beau_results" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The graphical representation of our proposed framework, namely background-agnostic feature extractor, which is composed of the blocks of pre-trained network, mask encoder and attention pooling layer. The red line means upsample using 1 × 1 convolution layer and a sigmoid activation. \( \mathcal{L} \) means the mean square error between mask prediction and mask label.
</div>

Extensive experimental results have demonstrated the superiority of our proposed framework.