---
layout: page
title: ProPredict
description: Agentic protein structure prediction
importance: 1
category: featured
---

**Stack:** Python, FastAPI, Celery, Redis, Postgres, Docker, Modal, LangGraph

**Code:** [github.com/Adi0521](https://github.com/Adi0521) <!-- swap in the repo URL -->

ProPredict predicts a protein's structure, runs physics simulation and mutation scoring on it, and lets an agent decide whether to accept the result, refine it, or escalate it.

### Results

- Raised structure-prediction accuracy (TM-score) from **0.50 to 0.87** across **88 benchmark targets** by adding retrieval-based conditioning

### How it works

- **Agent:** a LangGraph agent orchestrates structure prediction, physics simulation, and mutation scoring, then accepts, refines, or escalates each run. If the agent fails, it falls back to a deterministic loop.
- **Policies:** fast, accurate, and constraint-driven policies decide from ensemble uncertainty, pLDDT, and constraint checks: accept above pLDDT 80, refine at 60–80, escalate below 60.
- **Models:** ESMFold, Boltz, Chai, and GROMACS run in a multi-container setup supporting ligand docking, position-specific mutations (e.g., A12V), and iterative structure refinement.
- **Scoring:** a pipeline combining pLDDT, TM-score, and clash detection, with sha256 feature hashing keying a Redis cache across sequences and contexts.

### Infrastructure

- Two deployment modes: docker-compose locally (FastAPI + Celery/Redis + Postgres) and Modal GPUs for inference
- GitHub Actions CI and SSRF-guarded webhooks