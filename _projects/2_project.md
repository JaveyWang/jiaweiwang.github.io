---
layout: page
title: project 2
description: Graph Reasoning with Supervised Contrastive Learning for Legal Judgment Prediction
img: assets/img/4.jpg
importance: 2
category: work
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/GraSCL_LJP_task.png" title="GraSCL_LJP_task" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    An illustration of the LJP task which shows how the judge decides a legal case based on the fact. Each directed edge represents the pre-defined logical relation between labels.
</div>

To solve the problem of hierarchical multi-label classification, we proposed a GNN framework to model the label relationship based on the probabilistic decomposition of a directed acyclic graph (DAG). 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/GraSCL_framework.png" title="GraSCL_framework" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The illustration of our proposed framework, which is composed of a graph reasoning network and a node classification network. For a fact description, we first utilize a fact encoder to obtain its representations from raw text. Then we leverage the prior consistency of each label among different tasks based on a graph neural network. And the node classification network is proposed to predict the label distribution in terms of cross-entropy loss (node filled with color) and supervised contrastive loss (node defined as positive samples).
</div>

Each node in the DAG corresponds to a specific label, and the edges between the nodes correspond to the association between the labels. 

We further utilize the Supervised Contrastive Learning method to better consider the label relations. And the proposed model has achieved SOTA results on public datasets, which strongly proves its effectiveness.