---
layout: page
title: Coverage path planning
description: Offline area coverage path planning for GPS mobile robot
accolade: Best work-term report
img: /assets/img/jackal_thumb.jpg
github: https://github.com/ljazzal/area-coverage-nav
importance: 3
category: 2019
---

Following the integration of a new GPS sensor with the point-to-point navigation stack during my internship at Clearpath Robotics, I started experimenting with coverage path planning methods for mobile robots. Based on the popular Boustrophedon cell decomposition method, I implemented an offline coverage "path planning" algorithm to parse arbitrary polygons into a sequence of GPS waypoints which could then be passed to the mobile platform's navigation stack. The user need only select boundary points in a GUI with GPS images of the location to delineate the region of interest and the extented stack would compute the appropriate path segments, accounting for obstacles and non-convex angles.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/1.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/3.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/5.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>

