---
layout: page
title: reachability analysis
description: USC CURVE fellowship
img: assets/img/project1/hjreach.png
importance: 1
category: research
---

Faculty: Professor [Somil Bansal](https://smlbansal.github.io/)

PhD mentor : [Hao Wang](https://scholar.google.com/citations?user=W5WYNgkAAAAJ&hl=en&authuser=1)

Collaborator: [Peter Wang](https://pwang649.github.io/)

[[Project Github]](https://github.com/tianhao-stan-wu/deepreach)  &nbsp;&nbsp;&nbsp;&nbsp; [[paper]](https://arxiv.org/pdf/2312.17583v1)

<br>
This project focuses on Hamilton-Jacobi Reachability analysis. If you are unfamiliar with the topic, below are some good resources to get started.

1. [Overview of Reachability slides](https://drive.google.com/file/d/1DU8fz4mobCKtrXqi65xA5qDVV390ebaM/view) \[[Video](https://www.youtube.com/watch?v=iWsfc107nRc&list=PLrmdED6yqL3W6iCM3Vio3WzrsTTpkiluy&index=2)\]
 

2. [Ian Mitchell’s thesis](https://www.cs.ubc.ca/~mitchell/Papers/thesisMitchell.pdf) and [Somil Bansal’s thesis](https://drive.google.com/file/d/1iLV2MjHY1N8eDIJZ-Oja_gMQpsaGGdjq/view)

<br>
Because this project is quite theoretical, it took me (as a sophomore) almost a whole semester to just understand the mathematical formulation and background knowledge of Reachability. Then familiarized with two toolboxes [DeepReach](https://github.com/smlbansal/deepreach) and [HelperOC](https://github.com/HJReachability/helperOC) to solve Reachability problems.


To fully comprehend DeepReach, I first implemented a simple 2D system. This
[pdf](/assets/pdf/project1/2D_system.pdf) includes the problem description and the analytical solution of hamiltonian. Below are results obtained from DeepReach.

<br>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/project1/2D_value_function_goal.png" title="value function goal" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    BRT when target set is the goal set
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/project1/2D_value_function_unsafe.png" title="value function unsafe" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    BRT when target set is the failure set
</div>
<br>

Understanding DeepReach code and its implementation, I worked on a project that aims to improve the performance of DeepReach on high-dimensional Reachability problems by exploiting different activation functions in the DNN. 

<br>
Abstract: 

With the continuous advancement in autonomous
systems, it becomes crucial to provide robust safety guarantees
for safety-critical systems. Hamilton-Jacobi Reachability Analysis
is a formal verification method that guarantees performance
and safety for dynamical systems and is widely applicable to
various tasks and challenges. Traditionally, reachability problems
are solved by using grid-based methods, whose computational
and memory cost scales exponentially with the dimensionality of the system. To overcome this challenge, DeepReach, a
deep learning-based approach that approximately solves high-dimensional reachability problems, is proposed and has shown
lots of promise. In this paper, we aim to improve the performance
of DeepReach on high-dimensional systems by exploring different
choices of activation functions. We first run experiments on a
3D system as a proof of concept. Then we demonstrate the
effectiveness of our approach on a 9D multi-vehicle collision
problem.

<br>

The whole project is too much for this webpage. For more details, please check out the following:

1. [paper](https://arxiv.org/pdf/2312.17583v1) (most comprehensive)
2. [slides](/assets/pdf/project1/slides.pdf)
<br>

Here again, I want to express my deep appreciation for Professor Bansal and PhD candidate Hao Wang for their support throughout this research project. Without them, this piece of work would be impossible. Also, thanks everyone in the [SIA lab](https://smlbansal.github.io/sia-lab/people.html) for helping and supporting each other, making this research experience so wonderful!

<br>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/project1/lab_photo.jpg" title="photo" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    SIA Lab family
</div>
