---
layout: page
title: Entity Memory Database
description: PostgreSQL/Supabase project for canonical entities, generated dossiers, source provenance, activity timelines, commitments, evidence, RLS, and audit logs.
importance: 3
category: work
tech_stack: [PostgreSQL, Supabase, PL/pgSQL, RLS, n8n, LLM agents]
---

## Overview

Built a database-backed version of an LLM-maintained knowledge wiki for business entities and operating context, inspired by Andrej Karpathy's [LLM Wiki](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f) pattern.

Instead of saving generated knowledge as loose markdown pages, this project used PostgreSQL/Supabase to store entities, generated dossier pages, source provenance, activity logs, commitments, and handoff records across prospect, client, and operations workflows.

---

## What It Does

The project turns scattered business artifacts into records that can be queried, audited, and reused:

- Canonical entity records for people, companies, prospects, clients, and related business objects
- LLM-maintained profile and dossier records
- Source-level provenance for activities and notes
- Commitment tracking with evidence-based closure
- Cross-schema handoff from pipeline context into client and operations workflows
- Row-level security, audit triggers, and compatibility views for automation workflows

---

## Technical Focus

- PostgreSQL / Supabase schema design
- PL/pgSQL triggers and migration-safe compatibility layers
- Canonical entity resolution and backfills
- Row-level security and audit logging
- n8n and agent workflow integration
- Activity and commitment models tied back to source evidence

---

## Why It Matters

Handoffs often lose the useful details: discovery notes, entity facts, commitments, and evidence end up split across transcripts, calendars, forms, and automation logs. This project keeps those details in a structured database so agents and people can find the same source-backed record later.
