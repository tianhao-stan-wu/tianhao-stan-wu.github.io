---
layout: page
title: autonomous drone
description: UCI summer research
img: assets/img/project2/autodrone.jpg
importance: 2
category: research
---

Faculty: Professor [Marco Levorato](https://www.ics.uci.edu/~mlevorat/)

Project Director : Ian A. Harshbarger

Team: Yushi Lin, Jiajun Li, Purav Patel, Eric Qiu, Tianhao Wu

[[Project Github]](https://github.com/tianhao-stan-wu/UCI_Autonomous_Drone_Project)

<br>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/project2/overview.jpg" title="overview" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Project Overview
</div>
<br>

First, we familiarized ourselves with the working environment, including but not limited to Github repositories for UAVs, [dronekit documentation](https://dronekit-python.readthedocs.io/en/latest/), and Jetson Nano.

<br>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/project2/digitIO.jpg" title="digital IO" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Jetson Nano/CircuitPython documentation
</div>
<br>

Then, configured VL53L0X time of flight sensor, connected it with jetson nano, and adapted Python scripts to print distance data.

<br>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/project2/tfsensor.jpg" title="time of flight sensor" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/project2/board.jpg" title="breadboard" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    time of flight sensor &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; connect ToF sensor to Jetson Nano
</div>
<br>

Next, we built a target using cardboards and PVC pipes; collected, cleaned, and labeled a dataset of the target on Roboflow for training a YOLOv5 model.

<br>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/project2/target.jpg" title="target" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/project2/dataset.jpg" title="dataset" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    target &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; sample dataset
</div>
<br>

Validated the YOLOv5 model, successfully detected the target and the stop sign with high accuracy (over 90%). We further exploited this high accuracy by dynamically calculating the percentage of the target in images captured by the onboard webcam as a safety guarantee. 

<br>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/project2/test.png" title="validation" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    validation
</div>
<br>

Then, scripted a simulation using dronekit-silt, fixed bugs in our code, and optimized the algorithm. After trials and errors, we ran the simulation with Mission Planner and passed the test. Finally, we tested our drone in an open field.

<br>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/project2/simulation.jpg" title="simulation" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    simulation
</div>
<br>
