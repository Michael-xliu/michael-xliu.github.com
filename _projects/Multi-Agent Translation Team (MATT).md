---
layout: page
title: Multi-Agent Translation Team (MATT) - Published
description: Low-resource language translation project using LLM review, editing, and evaluation agents.
img: /assets/img/MATT/Architecture_logo.png
importance: 1
category: work
---

## Abstract

This paper introduces **Multi-Agent Translation Team (MATT)**, a workflow for refining English-to-low-resource language translations. The project tested LLM-based proofreading, editing, and evaluation roles across **Vietnamese**, **Hindi**, and **Malayalam**.

The workflow improved on the baseline model in the tested languages and was compared with Google Translate using automated scores and human review.

---

## Introduction

Many online resources are still hard to use for people who do not read English. Machine translation tools such as **Google Translate (GT)** help, but low-resource languages remain harder because there is less training data and more room for context to be lost.

---

## Why This Matters

- Only **15%** of the world speaks English, leaving a large share of online knowledge harder to access.
- Countries like **Vietnam** and **India**, with growing foreign investment, still face communication barriers tied to language access.
- In medical, legal, and research settings, **poor translation can create real risk**.

MATT uses separate agent roles so translation, review, editing, and scoring are handled as distinct steps.

---

## Architecture

MATT refines translation in two stages:

1. **Initial translation generation:** Uses **Llama 3.1** and the **Google Translate API**.
2. **Iterative refinement:** Uses proofreading, editing, and loss assessment agents.

**Components:**

- **Evaluation Coordinator:** Selects the strongest base translation.
- **Proofreader and Editor:** Review fluency, accuracy, style, and terminology.
- **Editor-in-Chief:** Scores **Loss in Translation (LiT)** and handles final review.

![Workflow Diagram](/assets/img/MATT/Architecture.png)

---

## Results

| Model | Vietnamese | Hindi | Malayalam |
|--------|------------|------|------------|
| **Baseline** | **0.2471** | **0.1390** | **0.0158** |
| **MATT** | **0.2952** | **0.1681** | **0.0231** |
| **Google Translate** | **0.3886** | **0.2548** | **0.0728** |

- MATT outperformed the baseline across all three tested languages.
- Human evaluations favored MATT over both GT and baseline models for fluency and context.

![Results Graph](/assets/img/MATT/Score.png)

---

## Takeaways

- **MATT improved translation quality** over the baseline in the tested low-resource settings.
- **GT remained strong** on direct word-to-word scores.
- **Human reviewers preferred MATT** in cases where fluency and context mattered more than literal overlap.

## Limitations

- API calls and repeated review steps add processing time.
- LLM outputs can vary between runs, so prompts and evaluation rules need to be stable.
- Some languages still need more training data for larger gains.

---

## Conclusion

MATT shows one way to use agent roles for translation review: generate a draft, critique it, revise it, and score what changed. The strongest result was not that agents replace machine translation, but that a review loop can catch context and fluency issues that a single-pass translation may miss.

---

View the full publication on [SMU Scholar](https://scholar.smu.edu/datasciencereview/vol8/iss3/3/).
