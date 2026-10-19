---
layout: page
title: Event-Driven Trading Bot
description: Autonomous news-to-trade pipeline for Kalshi · HackIllinois 2026
importance: 2
category: featured
---

**Stack:** Python, C++, Flask, React, Vite, Three.js, Modal, Groq

**Code:** [github.com/Adi0521](https://github.com/Adi0521) <!-- swap in the repo URL -->

A fully autonomous bot that reads the news, decides which prediction markets it affects, and trades on them. Built at HackIllinois 2026.

### Results

- Executed **200+ trades** at a **70%+ win rate** for $50+ net P&L
- **5–7 ms** order construction and signing in the C++ execution path

### Pipeline

1. **Ingest:** 25+ RSS feeds, deduplicated by URL hash so the same story never fires twice
2. **Match:** SentenceTransformers map each headline to candidate Kalshi tickers (minimum match confidence 0.40)
3. **Score:** FinBERT sentiment on Modal A10G GPUs (minimum score 0.70 to enter)
4. **Route:** ambiguous events go to Llama 3.3 70B via Groq for a second opinion
5. **Execute:** a C++ path issues RSA-PSS signed limit orders to Kalshi
6. **Exit:** a background sell-heartbeat watches open positions and closes them on sentiment reversal

### Deployment

Flask + server-sent events backend on Railway, React/Vite/Three.js dashboard on Vercel.
