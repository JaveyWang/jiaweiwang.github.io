---
layout: page
title: project 1
description: Visual Classification with Causal Concept Graph
img: assets/img/1.jpg
importance: 1
category: work
---

To consider the causal relationship between different labels for the visual classification task, a Causal Concept Graph (CCG) is established to explicitly model the relation of label concepts using the Structural Causal Model (SCM).

<div class="row">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/CCG1.png" title="CCG1" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/CCG2.png" title="CCG2" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
    This figure illustrates a causal concept graph about four interested labels, showing the causal relation of different labels.
</div>

The edge weights of CCG are estimated based on the Potential Outcome Model (POM), such as Propensity Score Matching and Inverse Probability of Weighting techniques. 

Based on this, a plug-in module, label-propagation graph neural network, is proposed to perform visual classification, which demonstrates its effectiveness compared to the traditional label-independent classification models.