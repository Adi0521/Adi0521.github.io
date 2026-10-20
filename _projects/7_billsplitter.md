---
layout: page
title: BillSplitter
description: C++ bill-splitting app with receipt OCR
importance: 7
category: more
---

**Stack:** C++17, Crow, PostgreSQL, Vue 3, Vite, Tailwind, Tesseract OCR

A bill-splitting app that reads the receipt for you, in active use among friend groups.

- **Backend:** a C++ REST API with object-oriented design that separates bills, line items, people, and split groups into distinct classes, persisted in PostgreSQL
- **OCR:** receipt scanning that drafts line items from common bill formats and screenshots, with automatic tip and tax calculation plus manual override
- **Balances:** a running balance per person within a split, with automatic cleanup when a group is deleted
