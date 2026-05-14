---
layout: page
title: Internal GenAI Platform
description: Internal GenAI platform with Open WebUI, AWS Bedrock, RAG, SSO, model routing, and SLO dashboards.
img: /assets/img/chatbot/WebUI.png
importance: 2
category: work
tech_stack: [Open WebUI, AWS Bedrock, PostgreSQL, pgvector, ECS, S3, FastAPI]
---

## Overview

Built an internal GenAI platform for investment and operations workflows. It combined Open WebUI, AWS Bedrock, RAG, SSO, model routing, a prompt/version registry, and SLO dashboards.

The platform supported **30+ active users**, **10k+ interactions**, roughly **99% uptime**, quarterly compliance log exports, and **30% faster investment and operations workflows**.

---

## Architecture

- **Interface:** Open WebUI
- **LLM layer:** AWS Bedrock with model routing
- **Retrieval:** Native RAG over internal documents and email-derived knowledge sources
- **Governance:** SSO, role-aware access, audit trails, and compliance log exports
- **Operations:** SLO dashboards for latency, cost, accuracy, and reliability
- **Prompt operations:** Prompt/version registry for controlled iteration and rollback

---

## Retrieval and Reliability

The retrieval layer used strict prompting, citations, fallback/no-answer behavior, and offline evaluation. Hybrid retrieval and reranking helped keep answers tied to source material.

---

## Impact

- Supported **30+ active users**
- Served **10k+ interactions**
- Maintained roughly **99% uptime**
- Accelerated investment and operations workflows by **30%**
- Enabled quarterly compliance log exports
- Reduced LLM operating cost through response caching and model routing

---

## Tools and Technologies

- AWS Bedrock
- Open WebUI
- PostgreSQL / pgvector
- ECS
- S3
- SSO
- Python
- FastAPI
- Docker
