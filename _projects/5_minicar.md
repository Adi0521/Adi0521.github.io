---
layout: page
title: Self-Driving MiniCar
description: Solo-built autonomous car with LiDAR + camera fusion
importance: 5
category: more
---

**Stack:** Python, C++, OpenCV, MATLAB Simulink


A solo, end-to-end build: I designed the chassis in CAD, sourced and soldered the components, wrote the control stack, validated it in MATLAB Simulink, and deployed it to embedded hardware.

- Fused LiDAR and camera frames as CNN input for obstacle detection and route correction
- Cut lap time on a 400 m course by **~4.5 seconds** through model compression and algorithmic optimization under embedded compute limits
