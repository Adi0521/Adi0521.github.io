---
layout: page
title: Distributed CPU Inference Cluster
description: Daisy-chained CPU nodes for running models locally
importance: 5
category: in progress
---

**Stack:** Ubuntu, Docker, MPI, Slurm, TCP sockets, PyTorch, NFS, Grafana, SimGrid

A cluster of daisy-chained CPU nodes for running models locally, without GPUs.

- **Networking and scheduling:** nodes communicate over TCP sockets and MPI, with Slurm job scheduling and a shared NFS file system
- **Runtime:** workloads run in Docker containers on Ubuntu with compiled kernels and a PyTorch runtime
- **Monitoring:** Grafana dashboards across the cluster
- **Validation:** simulating the design in SimGrid across 8 nodes before building it out
