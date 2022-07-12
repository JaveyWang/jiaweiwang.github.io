---
layout: page
title: project 4
description: REAL2 - An End-to-end Memory-augmented Solver for Math Word Problems (NeurIPS Workshop)
img: assets/img/5.jpg
# redirect: https://unsplash.com
importance: 4
category: work
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/REAL2_framework.png" title="REAL2_framework" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The illustration of our proposed REAL2 framework, which is composed of two stages. In the first stage, for an unsolved problem \( X \), we first use a Word2Vec-based retriever to pre-ranking the most similar N candidate questions from the question bank. And the K similar questions are re-ranking based on the candidate questions and a trainable memory module. In the second stage, the token distributions of solution are generated based on the unsolved problem with its retrieved questions, and the aggregated token distribution is the final solution of the unsolved problem.
</div>

In order to solve the problems of the previous template-based two-stage generation method, we innovatively designed an algorithm for solving math word problems based on a memory-augmented solver. The proposed algorithm achieves SOTA performance on the Math23K benchmark, which also has a specific few-shot learning ability. (EMNLP; NeurIPS)
