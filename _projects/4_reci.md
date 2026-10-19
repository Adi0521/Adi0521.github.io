---
layout: page
title: Reci
description: Social recipe platform · 3rd place, Research Park Hackathon
importance: 4
category: more
---

**Stack:** Next.js 16, TypeScript, Tailwind v4, FastAPI, SQLAlchemy 2, Supabase

**Code:** [github.com/Adi0521](https://github.com/Adi0521) <!-- swap in the repo URL -->

A full-stack social platform for sharing and rating recipes. Placed **3rd at the Research Park Hackathon**.

- FastAPI + SQLAlchemy 2 backend and Next.js App Router frontend, both deployed as serverless Vercel projects
- Supabase Auth with JWTs and username-or-email login; ~100 seeded public recipes in Supabase Postgres, using NullPool for serverless connections
- Social layer with star-rating reviews, a friends/followers graph, a ranked leaderboard with tier filters, and user profiles
