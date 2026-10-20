---
layout: page
title: Self-Driving MiniCar
description: Solo-built autonomous car with LiDAR + camera fusion
importance: 10
category: more
---

**Stack:** Python, C++, OpenCV, MATLAB Simulink

A solo, end-to-end build: I designed the chassis in CAD, sourced and soldered the components, coded the algorithms, validated everything in MATLAB Simulink, and deployed it on embedded hardware.

- Preprocessed LiDAR and camera frames and used a CNN for obstacle detection, route correction, and sensor fusion
- Improved times around a 400-meter route by **~4.5 seconds** through model compression and algorithmic optimization for embedded constraints
