---
layout: page
title: Financial Roaster
description: A small AWS Bedrock app that reviews spending data with four parallel agents and returns a roast-style financial summary.
img: /assets/img/financial-roaster/preview.png
importance: 3
category: fun
---

## Try It Out

[Launch Financial Roaster](https://financial-roaster.onrender.com/)

---

## Overview

Financial Roaster reviews spending data and turns it into a roast-style summary. Four agents handle cleanup, pattern detection, risk checks, and the final write-up.

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

The app uses four agents:

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
- **Mobile responsive**: Works on phone and desktop screens
- **Cost efficient**: ~$0.01 per analysis

---

## Deployment

- **Platform**: Render (auto-deploys from GitHub)
- **Environment**: Python 3.11 + AWS Bedrock
- **Caching**: File-hash based caching to avoid redundant processing
