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

Following the integration of a new GPS sensor with the point-to-point navigation stack during my internship at Clearpath Robotics, I started experimenting with coverage path planning methods for mobile robots. Based on the popular [Boustrophedon cell decomposition method](https://asset-pdf.scinapse.io/prod/1590932131/1590932131.pdf), I implemented an offline coverage ``path planning'' algorithm to parse arbitrary polygons into a sequence of GPS waypoints which could then be passed to the mobile platform's navigation stack. The user need only select boundary points in a GUI with GPS images of the location to delineate the region of interest and the extented stack would compute the appropriate path segments, accounting for obstacles and non-convex angles.
