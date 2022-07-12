---
layout: page
title: project 5
description: MOC - Measuring the Originality of Courseware in Online Education Systems. (ACMMM Oral paper)
img: assets/img/10.jpg
importance: 5
category: work
---

In online education systems, the courseware plays a pivotal role in helping educators present and impart knowledge to students. The originality of courseware heavily impacts the choice of educators, because the teaching content evolves and so does courseware.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/MOC_courseware.png" title="MOC_courseware" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The illustration of a courseware, which is composed of visual and textual content and is continuously updated.
</div>

However, how to measure the originality of a courseware is a challenging task, due to the lack of labels and the difficulty of quantification. To this end, we contribute a similarity ranking-based unsupervised approach to measure the originality of a courseware.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/MOC_overview.png" title="MOC_overview" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The graphical representation of our propose framework, which is composed of \emph{Deep Visual-text Embedding}, \emph{Variable-length Vectors Integration}, and \emph{Mutual Information Maximization}.
</div>

 In particular, we first exploit a pre-trained deep visual-text embedding to obtain the representations of images and texts in a local manner. Next, inspired by the design of capsule neural network, a vector-based pooling network is proposed to learn multimodal representations of images and texts. Finally, we propose a Discriminator to optimize the model by maximizing the mutual information between local features and global features in an unsupervised manner.
 
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/MOC_flowchart.png" title="MOC_flowchart" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The illustration of how to evaluate the framework.
</div>

  To evaluate the performance of our proposed model, we further subtly collect a dataset for evaluating the originality of courseware by treating sequential versions of each courseware as ranking lists. Therefore, the learning-to-rank scheme can be utilized to evaluate the similarity-based ranking performance. Extensive experimental results have demonstrated the superiority of our proposed framework as compared to other state-of-the-art competitors.