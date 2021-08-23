---
layout: page
title: It's all about attitude...
description: Monocular spacecraft pose estimation from a single image
img: /assets/img/attitude.png
github: https://github.com/ljazzal/spacecraft-pose-estimation
pdf: /assets/pdf/aer1515_final_report_2020.pdf
importance: 2
category: 2020
---
<div class="publications">
  {% bibliography -f papers -q @*[year={{2020}}]* %}
</div>

Launching anything in orbit is expensive and access is limited if not impossible once it’s up there. There has been a lot of interest in recent years, with projects like OSAM and ClearSpace, in adding active maintenance to the satellite life cycle, potentially expanding the life expectancy of space assets. Whether it be refueling, repairs or even removal, the maintenance of space vehicles and their orbital environment is seen as a crucial endeavour. Typically, the target satellite is known beforehand and a detailed 3D model of the vehicle is available for close-proximity operation. However, in the case of space debris or defunct satellites, exact models might not be available, warranting the use of generalizable techniques that only rely on scene information. Perception algorithms such as object detection and pose estimation could provide valuable estimates of the state of the target object.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/high_level.png' | relative_url }}" alt="" title="pipeline"/>
    </div>
</div>
<div class="caption">
    High level pipeline for an on-board pose estimation algorithm
</div>

The Kelvins Satellite Pose Estimation Challenge was designed to evaluate vision-based approaches to 6D pose estimation. The challenge was based on the SPEED dataset from the Stanford Space Rendezvous Lab, which provides fixed camera intrinsics and groundtruth pose in the form of a translation vector and unit quaternion vector, relative to the camera (assumed to be on-board a neighboring spacecraft).

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/cnn_arch.png' | relative_url }}" alt="" title="CNN architecture"/>
    </div>
</div>
<div class="caption">
    CNN architecture for the full 6D pose estimation from a single image
</div>

This challenge was undertaken as the final project in a course on perception for robotics. The goal was to determine the position and orientation of the target spacecraft from a single image. In the interest of simplicity, an end-to-end approach was adopted, based on a common backbone (`ResNet-34`) and separate branches for the translation and orientation regression. Instead, emphasis was put on the comparison of three different attitude descriptors: unit quaternions, Euler angles and the Euler axis-angle representation. We were interested to determine if any particular attitude descriptor presented advantages in the direct regression of the orientation degrees of freedom.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/attitude_descriptors.png' | relative_url }}" alt="" title="CNN architecture"/>
    </div>
</div>
<div class="caption">
    Comparison of orientation regression based on three different attitude descriptors
</div>
