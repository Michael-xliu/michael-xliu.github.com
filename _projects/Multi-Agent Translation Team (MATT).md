---
layout: page
title: Multi-Agent Translation Team (MATT)
description: Enhancing Low-Resource Language Translation through Multi-Agent Workflow
img: /assets/img/MATT/Architecture.png
importance: 1
category: work
---

# Multi-Agent Translation Team (MATT)

## Enhancing Low-Resource Language Translation through Multi-Agent Workflow

This document introduces the **Multi-Agent Translation Team (MATT)**, a novel approach to enhancing translations from English to low-resource languages using multi-agent workflows. Inspired by human collaborative problem-solving, MATT integrates advanced techniques with tools like **GPT-4o** and **Llama 3.1** to achieve high-quality translation outputs.

---

## Abstract

Like humans, **Large Language Models (LLMs)** benefit from revision and refinement, especially for complex tasks. This study showcases a multi-agent workflow that assigns specific roles—translator, evaluation coordinator, and editor—to refine translations iteratively. MATT achieves notable improvements, particularly in translating to languages like Vietnamese, Hindi, and Malayalam.

---

## Introduction

Language is essential for sharing and preserving knowledge. However, only a fraction of the world's languages are well-represented online. MATT addresses these disparities by combining **Google Translate (GT)** and advanced LLMs for better accuracy and cultural nuance.

**Key Goals:**
- Enhance translations for low-resource languages.
- Mimic human collaborative problem-solving through LLM-powered agents.

---

## Methods

### Multi-Agent Workflow Layers
1. **Initial Translation Generation:**
   - Llama 3.1 and GT API are used for baseline translations.
2. **Translation Refinement:**
   - Roles like proofreader and editor improve fluency, accuracy, style, and terminology.
3. **Iterative Feedback Loop:**
   - Refinement continues until the translation loss is under a 10% threshold.

### Metrics
- **BLEU Scores:** Quantitative measure of translation accuracy.
- **Human Evaluation:** Gold standard for assessing translation quality.
- **LLM Evaluation:** Utilizes models like GPT-4o for additional insights.

---

## Results

- **Comparison with Baseline:** MATT outperforms initial workflows across all evaluation metrics.
- **Language-Specific Findings:**
  - **Vietnamese:** Significant improvement in human-preferred translations.
  - **Hindi:** Noticeable gains in fluency and cultural relevance.
  - **Malayalam:** Challenges remain due to limited training data.

---

## Limitations and Future Work

### Challenges:
- High computational cost.
- Variability in LLM outputs.
- Limited data for low-resource languages.

### Future Directions:
- Expand to more languages and domains.
- Integrate human-agent collaboration.
- Improve metrics for evaluating cultural adaptability.

---

For further details, view the full article on [SMU Scholar](https://scholar.smu.edu/datasciencereview).
