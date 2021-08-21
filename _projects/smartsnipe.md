---
layout: page
title: SmartSnipe shooter tutor
description: >
    "You miss 100% of the shots you don't take." - Wayne Gretzky
accolade: Best prototype quality
img: /assets/img/demo.gif
github: https://github.com/ljazzal/smartsnipe-obc
importance: 3
category: 2020
---

SmartSnipe is a smart hockey "shooter tutor" that can be attached to any hockey net to enhance the shooting practice experience. By leveraging actuators mounted on the board, the slots are remotely controlled to simulate goal scoring opportunities, while a player-facing camera, a speed gun and various detection sensors are fused to produce performance indicators and provide feedback to the player. Action recognition via CNN-based pose estimation is being researched to infer when a player is in a shooting position. The results shown below have been obtained with a modified OpenPose library running on an NVIDIA Jetson TX1 with a Kinectv1 camera.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/smartsnipe_arch.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    The software architecture of the SmartSnipe system implemented with ROS
</div>

At the 2020 Mechatronics Engineering Capstone Design Symposium (University of Waterloo), the project was co-awarded __Best prototype quality__.
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/smartsnipe_poster.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    Capstone symposium poster
</div>
