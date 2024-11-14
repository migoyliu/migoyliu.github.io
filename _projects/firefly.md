---
layout: page
title: Fire Ember Detection
description: Wildfire simulation rendering, data collection pipeline in Unreal Engine, tiny ember object detection.
img: assets/img/firefly.jpg
importance: 2
category: work
---

After witnessing multiple wildfires in LA, in the summer of 2022, I joined <a href="https://sites.usc.edu/eessc/">USC E2S2C</a> Group as an <a href="https://viterbischool.usc.edu/news/2022/02/usc-and-amazon-announce-joint-summer-research-program-for-undergraduates/">Amazon SURE</a> Research Fellow to advance wildfire management with simulation and machine learning. 

During wildfires, embers can travel miles in wind and cause up to 90% of home ignition. The ultimate goal of this project is to detect and extinguish them with UAV before they spread the fire. While there are many datasets for fire and smoke detection, there is none for tiny ember, making them infessible to detect. This motivated us to create FireFly, a synthetic dataset that enables zero-shot ember detection in real wildfire scenarios.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/firefly.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true%}
    </div>
</div>
<div class="caption">
    Inference on real wildfire at Sycan Marsh Preserve, Oregon. Video provided by U.S. Department of Agriculture.
</div>

For more technical details, please refer to <a href="https://arxiv.org/pdf/2308.03164">our paper</a>. 