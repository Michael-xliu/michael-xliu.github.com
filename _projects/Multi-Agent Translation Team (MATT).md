---
layout: page
title: Multi-Agent Translation Team (MATT)
description: Enhancing Low-Resource Language Translation through Multi-Agent Workflow
img: /assets/img/MATT/Architecture.png
importance: 1
category: work
---


# Multi-Agent Translation Team (MATT): Enhancing Low-Resource Language Translation

![Header Image Placeholder](./header-image.png)

## 📌 Abstract

Large language models (LLMs) benefit from revision and refinement, much like human collaborators in complex tasks requiring critical thinking. This paper introduces **Multi-Agent Translation Team (MATT)**—a sophisticated, iterative multi-agent workflow that refines English-to-low-resource language translations. Leveraging **LLMs, Google Translate (GT), and role-based agents**, MATT systematically enhances translation accuracy for **Vietnamese, Hindi, and Malayalam**. 

This study presents a pioneering approach that outperforms baseline models by integrating **evaluation coordinators, proofreaders, editors, and iterative loss minimization strategies**. The results highlight **MATT's ability to deliver improved fluency, accuracy, and contextual adaptation** compared to conventional machine translation models.

---

## 📖 Introduction

![Language Diversity Image Placeholder](./language-diversity.png)

Language serves as a **fundamental cultural bridge**, yet the majority of online content remains inaccessible to non-English speakers. Machine translation tools such as **Google Translate (GT)** have made strides, but they struggle with **low-resource languages**, where linguistic nuances and contextual subtleties are harder to encode. 

### 🌍 Why This Matters
- Only **15%** of the world speaks English, leaving vast knowledge inaccessible.
- Countries like **Vietnam and India**, with growing foreign investments, face communication barriers due to limited English proficiency.
- In medical, legal, and research domains, **poor translation can lead to significant consequences**.

MATT addresses these challenges by integrating **multi-agent workflows**, ensuring translations maintain **semantic integrity, fluency, and cultural appropriateness**.

---

## 🔬 Methodology

### 🚀 The MATT Architecture

MATT refines translation in a **two-layered process**:
1. **Initial Translation Generation**: Utilizes **Llama 3.1 and Google Translate API**.
2. **Iterative Translation Refinement**: Involves **proofreading, editing, and loss assessment** by LLM-powered agents.

**Key Components:**
- **Evaluation Coordinator** – selects the most reliable base translation.
- **Proofreader & Editor** – refine fluency, accuracy, style, and terminology.
- **Editor-in-Chief** – quantifies **Loss in Translation (LiT)** and ensures quality control.

![Workflow Diagram](./assets/img/MATT/Architecture.png)

---

## 📊 Results & Performance Analysis

### ✨ BLEU Score Comparison
| Model | Vietnamese | Hindi | Malayalam |
|--------|------------|------|------------|
| Baseline | 0.2471 | 0.1390 | 0.0158 |
| **MATT** | **0.2952** | **0.1681** | **0.0231** |
| Google Translate | 0.3886 | 0.2548 | 0.0728 |

- MATT **outperforms the baseline** consistently across all languages.
- **Human evaluations** favor MATT over both **GT and baseline models** in fluency and contextual adaptation.

![Results Graph Placeholder](./assets/img/MATT/Score.png)

---

## 🤔 Discussion

### 📌 Key Takeaways
- **MATT significantly improves translation quality** by leveraging structured **multi-agent collaboration**.
- **GT remains stronger in high-resource settings**, but MATT **surpasses it in nuanced, low-resource translations**.
- **Human preference aligns with MATT**, while **BLEU scores favor GT** due to direct word-to-word comparisons.

### 🚧 Limitations
- Computational cost and API dependencies can **increase processing time**.
- LLMs may exhibit **inconsistencies**, requiring improved **prompt engineering**.
- Some languages still require **more training data for significant gains**.

---

## 📌 Conclusion

MATT represents a significant leap forward in **low-resource language translation**, demonstrating how **multi-agent systems can enhance LLM-based translation** workflows. By combining **structured evaluation, iteration, and refinement**, MATT provides a robust **alternative to traditional MT models**, achieving improved **accuracy, fluency, and contextual integrity**.

---

For further details, view the full publication on [SMU Scholar](https://scholar.smu.edu/datasciencereview), currently under review.
