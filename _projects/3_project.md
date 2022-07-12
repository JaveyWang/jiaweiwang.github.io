---
layout: page
title: project 3
description: Recall and Learn - A Memory-augmented Solver for Math Word Problems (EMNLP)
img: assets/img/7.jpg
importance: 3
category: work
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/REAL_teaser_figure.png" title="REAL_teaser_figure" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Illustration of our proposed framework for solving math word problems in a recall and learn manner.
</div>

In this article, we tackle the math word problem, namely, automatically answering a mathematical problem according to its textual description. Although recent methods have demonstrated their promising results, most of these methods are based on template-based generation scheme which results in limited generalization capability. 

To this end, we propose a novel human-like analogical learning method in a recall and learn manner. Our proposed framework is composed of modules of memory, representation, analogy, and reasoning, which are designed to make a new exercise by referring to the exercises learned in the past. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/REAL_framework.png" title="REAL_framework" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The illustration of our proposed REAL framework, which is composed of modules of memory, representation, analogy and reasoning. For an unsolved problem \( X \), we first use maximum inner product search to find a similar question \( Z \) from the memory module. And then the solution is generated with the copy mechanism in an analogical manner.
</div>

Specifically, given a math word problem, the model first retrieves similar questions by a memory module and then encodes the unsolved problem and each retrieved question using a representation module. 

Moreover, to solve the problem in a way of analogy, an analogy module and a reasoning module with a copy mechanism are proposed to model the interrelationship between the problem and each retrieved question. 

Extensive experiments on two well-known datasets show the superiority of our proposed algorithm as compared to other state-of-the-art competitors from both overall performance comparison and micro-scope studies.