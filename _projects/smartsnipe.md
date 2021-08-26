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

SmartSnipe is a smart hockey "shooter tutor" that can be attached to any hockey net to enhance the shooting practice experience. By leveraging actuators mounted on the board, the slots are remotely controlled to simulate goal scoring opportunities, while a player-facing camera, a speed gun and various detection sensors are fused to produce performance indicators and provide feedback to the player. Action recognition via CNN-based pose estimation is being researched to infer when a player is in a shooting position. The results below have been obtained with a Kinect camera and a modified OpenPose library running on an NVIDIA Jetson TX1.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" style="margin-left: auto; margin-right: auto;" src="{{ '/assets/img/demo_gate.gif' | relative_url }}" alt="" title="SmartSnipe front"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" style="margin-left: auto; margin-right: auto;" src="{{ '/assets/img/demo.gif' | relative_url }}" alt="" title="live pose estimation"/>
    </div>
</div>
<div class="caption">
    The doors are remotely controlled from a mobile application (e.g., by the coach) for a predefined amount of time to simulate in-game scoring opportunities. Training sessions are recorded in order to analyze the player's shooting pose (offline) 
</div>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/smartsnipe_arch.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    The software architecture of the SmartSnipe system implemented with ROS
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/smartsnipe_poster.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    At the 2020 Mechatronics Engineering Capstone Design Symposium (University of Waterloo), the project was co-awarded "Best prototype quality".
</div>
