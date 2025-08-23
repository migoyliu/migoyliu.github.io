---
layout: page
title: Offroad Autonomy
description: A full off-road autonomous navigation system capable of driving in complete darkness. From cross-modality calibration to stereo vision and traversability estimation, this project pushed the limits of off-road autonomy.
img: assets/img/offroad.jpeg
importance: 1
category: work
---
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/offroad_night.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Offroad ATV driving in darkness at our test site, Gascola, PA.
</div>

Bringing a full-scale ATV into unstructured terrain at night is not easy. At the AirLab, I've had the opportunity to work with an incredible team to tackle this challenge, contributing across the entire stack from sensor integration, to perception, autonomy, and field testing.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/cross_calibration_board.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/thermal_mapping.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/thermal_costmap.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: Custom cross-modality calibration board. Middle: Thermal-LiDAR mapping. Right: Traversability costmap.
</div>

One of the first important steps in integrating new sensors is calibration. With a detailed material study to ensure visibility across modalities, we designed a custom calibration board capable of calibrating RGB (mono/stereo), thermal (mono/stereo), and multiple LiDARs. A lot of effort went into sensor drivers, time synchronization, and calibration, but these steps were crucial for achieving accurate sensor fusion and robust multi-modal autonomy.

On top of the foundation, we fused thermal data with LiDAR-SLAM to enable thermal mapping. We then leverage visual foundation model (VFM) and advanced image preprocessing to extract self-supervised features, which we combined with inverse reinforcement learning to estimate traversability. This allows us to bring autonomy into conditions where visible light fails, such as nighttime and smoke-filled environments.

Looking ahead, we are working to reduce the system’s reliance on LiDAR. We are developing a stereo VIO pipeline with learned uncertainty with the goal of enabling fully passive autonomy.


For more technical details, please refer to <a href="https://theairlab.org/offroad/">our project website</a>. 

Media Coverage:
- <a href="https://www.ri.cmu.edu/taking-autonomous-driving-off-road/">CMU RI News: Taking Autonomous Driving Off-Road</a>
- <a href="https://triblive.com/business/technology/cmus-tartan-driver-takes-autonomous-driving-off-pittsburghs-beaten-path">TRIB LIVE: CMU's Tartan Driver takes autonomous driving off Pittsburgh's beaten path</a>
- <a href="https://www.post-gazette.com/business/tech-news/2025/05/09/self-driving-atv-carnegie-mellon-university-airlab-demo/stories/202505080115">Pittsburgh Post-Gazette: Self-driving ATVs — designed at CMU — are made to help in times of disaster</a>
- <a href="https://www.wtrf.com/news/carnegie-mellon-university-students-are-on-the-road-to-success-with-self-driving-atv/">WTRF: Carnegie Mellon University students are on the road to success with self-driving ATV</a>