---
layout: page
title: ProPredict
description: Agentic protein structure refinement service
importance: 1
category: featured
---

**Stack:** Python, FastAPI, Celery, Redis, Postgres, Docker, Modal, GitHub Actions

**Code:** [github.com/Adi0521](https://github.com/Adi0521) <!-- swap in the repo URL -->

ProPredict predicts a protein's structure, then lets an agent iteratively refine it until the model is confident in the result.

### Results

- Raised mean pLDDT from **68.9 to 88.2** across the benchmark set through agent-driven refinement
- Benchmarked on **88 CASP15 targets**: TM-score 0.503 without MSA and **0.871 with MSA**
- Validated the ProteinMPNN mutation scorer against ProteinGym deep mutational scanning data, reaching **Spearman ρ 0.756** on the best-performing assay

### How it works

- **Agent loop:** a tool-use agent with 8 tools (analyze, relax, simulate, re-fold, scan and apply mutations, accept, escalate) refines structures autonomously, with a deterministic threshold fallback when the agent is disabled
- **Prediction:** ESMFold and Boltz-2 backends with multi-seed ensemble alignment, measuring per-residue Cα RMSD disagreement; ProteinMPNN mutation scoring is reproducible across 8 seeded decoding orders
- **Environment as input:** pH-dependent protonation via PropKa, membrane embedding via insane.py, and ligand docking via GNINA/Vina with ACPYPE/OpenFF parameterization
- **Simulation:** dual MD engines (OpenMM and GROMACS) with automated trajectory validation that catches NaNs, RMSD blowups, and radius-of-gyration divergence

### Infrastructure

- Dual-mode deployment: docker-compose (FastAPI + Celery/Redis + Postgres) locally, Modal A10G GPUs for production Boltz-2 inference
- Redis caching keyed on sha256 feature hashes, webhook callbacks with SSRF protection, and CI through GitHub Actions
