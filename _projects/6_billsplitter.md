---
layout: page
title: BillSplitter
description: Receipt OCR and running group balances
importance: 6
category: more
---

**Stack:** Next.js, Supabase, Google Vision API


A bill-splitting app that reads the receipt for you.

- Receipt OCR through Google Vision API that handles common bill formats and screenshots, with automatic tip and tax allocation plus manual override
- Running per-person balances scoped to a group, with Supabase auth, persistent storage, and automatic cleanup when a group is deleted
