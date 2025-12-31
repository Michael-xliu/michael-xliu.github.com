---
layout: page
title: Financial Roaster
description: An AI-powered financial analysis tool using AWS Bedrock and multi-agent orchestration to analyze spending habits with 4 specialized AI agents working in parallel.
img: /assets/img/financial-roaster/preview.png
importance: 3
category: fun
---

## Try It Out

[Launch Financial Roaster](https://financial-roaster.onrender.com/)

---

## Overview

Financial Roaster is an AI-powered tool that analyzes your spending data and delivers personalized, humorous feedback on your financial habits. It uses a multi-agent architecture to provide comprehensive analysis.

---

## Tech Stack

- **AI Engine**: AWS Bedrock + Claude 3 Haiku
- **Workflow**: LangGraph + Agent Core
- **Backend**: FastAPI (Python)
- **Frontend**: HTML/CSS/JavaScript
- **Deployment**: Render
- **OCR**: PyMuPDF + EasyOCR

---

## Multi-Agent Architecture

The system uses 4 specialized AI agents that work together:

### 1. The Accountant
- Cleans and normalizes transaction names
- Categorizes uncategorized transactions
- Flags data quality issues

### 2. The Detective
- Identifies recurring subscriptions
- Detects spending patterns and trends
- Highlights frequent merchants

### 3. The Risk Manager
- Identifies potential overdraft behavior
- Flags impulse purchase patterns
- Detects concerning spending habits

### 4. The Judge
- Calculates an overall financial health score (0-100)
- Synthesizes findings from other agents
- Generates the final analysis

---

## Parallel Processing

Agents run concurrently using Python's ThreadPoolExecutor, reducing analysis time by approximately 50%:

```python
with ThreadPoolExecutor(max_workers=3) as executor:
    detective_future = executor.submit(find_patterns)
    risk_manager_future = executor.submit(assess_risks)
    judge_future = executor.submit(calculate_chaos)
```

---

## Key Features

- **Multi-format input**: Supports CSV, PDF, images, and manual text entry
- **Smart parsing**: Combines regex and AI for accurate data extraction
- **Interactive results**: 3D flip cards for shareable output
- **Mobile responsive**: Optimized for all device sizes
- **Cost efficient**: ~$0.01 per analysis

---

## Deployment

- **Platform**: Render (auto-deploys from GitHub)
- **Environment**: Python 3.11 + AWS Bedrock
- **Caching**: File-hash based caching to avoid redundant processing