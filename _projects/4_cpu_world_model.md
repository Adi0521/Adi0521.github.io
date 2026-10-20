---
layout: page
title: CPU World Model Distillation
description: Running a diffusion world model entirely on CPU
importance: 4
category: in progress
---

**Stack:** Python, PyTorch, ONNX Runtime, DIAMOND, Atari Breakout

I'm distilling DIAMOND's pretrained Breakout diffusion world model into a student that runs entirely on CPU. An RL agent can then train on CPU-generated rollouts while the GPU handles distillation and policy updates.

### Approach

- **Optimization ladder:** a cheapest-first sequence of optimizations, each benchmarked as its own variant: batched inference, torch.compile and ONNX Runtime export, static INT8 quantization, network distillation, and consistency-style sampling-step distillation
- **Training loop:** a batched vector-environment adapter feeds DIAMOND's actor-critic learner, with a CPU throughput target derived from the transition budget a GPU reference agent needs to beat random

### Evaluation plan

- Multi-horizon dynamics validation with pixel-level event detectors
- 5-seed bot comparisons in real Breakout, with bootstrap confidence intervals against the GPU reference
