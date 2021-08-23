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

This research project was taken up on the side while interning at Clearpath Robotics. The original task involved the integration of a new GPS sensor with the Jackal UGV, the smalles outdoor UGV of the fleet. Given a smaller body, RTK GPS solutions are limited on such a platform and localization accuracy can be affected as a result.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/coverage_og_task.png' | relative_url }}" alt="" title="what I was supposed to work on"/>
    </div>
</div>
<div class="caption">
    Original sensor integration task and preliminary results
</div>

Once the new sensor had been integrated and localization results were satisfactory, I started experimenting with coverage path planning methods for outdoor mobile robots. Based on the popular [Boustrophedon cell decomposition method](https://asset-pdf.scinapse.io/prod/1590932131/1590932131.pdf), an offline coverage "path planning" algorithm was implemented to parse arbitrary polygons into a sequence of GPS waypoints which could then be passed to the mobile platform's navigation stack. The user need only select boundary points in a GUI with GPS images of the location to delineate the region of interest and the extended stack would compute the appropriate path segments, accounting for obstacles and non-convex angles.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/gazebo.png' | relative_url }}" alt="" title="simulation"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/angled_coverage.png' | relative_url }}" alt="" title="angled coverage"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/obstacle.png' | relative_url }}" alt="" title="obstacle"/>
    </div>
</div>
<div class="caption">
    The coverage path could be inspected in Gazebo before deployment (left), as the control interface provided an update of the coverage progress (middle, right)
</div>
