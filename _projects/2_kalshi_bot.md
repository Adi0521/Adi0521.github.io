---
layout: page
title: KalshiBot
description: Event-driven trading bot · HackIllinois 2026
importance: 2
category: featured
---

**Stack:** Python, C++, SQL, Flask, React, Modal, FinBERT, Groq

**Code:** [github.com/Adi0521](https://github.com/Adi0521) <!-- swap in the repo URL -->

A fully autonomous bot that reads the news, decides which prediction markets it affects, and trades on them with live capital. Built at HackIllinois 2026.

### Results

- Executed **200+ trades** at a **70%+ win rate** for $50+ net profit
- **5–7 ms** order construction and signing in the C++ execution layer

### Pipeline

1. **Ingest:** 25+ RSS feeds, deduplicated by URL hash so the same story never fires twice
2. **Match:** SentenceTransformers map each headline to candidate Kalshi tickers (minimum ticker confidence 0.40)
3. **Score:** FinBERT sentiment on Modal A10G GPUs (minimum score 0.70)
4. **Route:** ambiguous events go to Llama 3.3 70B via Groq for signal routing
5. **Execute:** a C++ layer issues RSA-PSS signed limit orders, enforcing stop-loss, max buy-in, and sell targets
6. **Exit:** a background sell heartbeat monitors positions and closes them on sentiment reversal

### Deployment

Trade and user data stored in SQL. Flask + server-sent events backend on Railway, React + Vite + Three.js frontend on Vercel.