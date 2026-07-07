---
layout: post
title: "Venice Beach: Sunset"
date: 2026-07-05 16:03:00
description:
categories: life
images:
  compare: true
  slider: true
---

<style>
.photo-gallery {
  width: 600px;
  margin: 2rem auto;
}

.photo-gallery swiper-container {
  width: 100%;
}

.photo-gallery img {
  width: 100%;
  height: auto;
  display: block;
}
</style>



<swiper-container keyboard="true" navigation="true" pagination="true" pagination-clickable="true" pagination-dynamic-bullets="true" rewind="true">
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/post-2026-07-05/venice-2.jpg" class="img-fluid rounded z-depth-1" %}</swiper-slide>
</swiper-container>



<div class="photo-gallery">
<swiper-container keyboard="true" navigation="true" pagination="true" pagination-clickable="true" pagination-dynamic-bullets="true" rewind="true">
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/post-2026-07-05/venice-7.jpg" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/post-2026-07-05/venice-6.jpg" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/post-2026-07-05/venice-8.jpg" class="img-fluid rounded z-depth-1" %}</swiper-slide>
</swiper-container>
</div>



<img-comparison-slider>
  {% include figure.liquid path="assets/img/post-2026-07-05/venice-5.jpg" class="img-fluid rounded z-depth-1" slot="first" %}
  {% include figure.liquid path="assets/img/post-2026-07-05/venice-5-color.jpg" class="img-fluid rounded z-depth-1" slot="second" %}
</img-comparison-slider>
