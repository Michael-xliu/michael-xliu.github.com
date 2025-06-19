---
layout: page
title: Large Language Models Pokémon Battle Arena
description: Claude 4 vs GPT-4.1 vs Gemini 2.5 Flash vs Human in AI Pokémon Battle
img: /assets/img/pokemon_ai_battle/pokemonarena.png
importance: 5
category: AI Projects
---

## Introduction

In this project, I developed a fully automated Pokémon battle arena to rigorously benchmark several leading large language models (LLMs) in a high-pressure, multi-turn strategic game environment. The core objective: test their tactical reasoning, adaptive planning, risk management, and agentic autonomy — skills essential for advanced AI systems.

### Competitors
- **Claude 3.7** (Anthropic, via AWS Bedrock)
- **Claude 4** (Anthropic, via AWS Bedrock)
- **GPT-4.1** (OpenAI, via OpenAI API)
- **Gemini 2.5 Flash** (Google, via Gemini API)
- **Human (myself, playing manually via custom interface)**

All battles ran under identical conditions using Pokémon Showdown’s **gen9randombattle** format, ensuring randomized but balanced teams across all nine generations of Pokémon. No pre-selected teams or setups — only pure in-the-moment decision-making.

---

## Technology Stack

- **poke-env** — Python battle simulation framework
- **AWS Bedrock API** — Claude model integration
- **OpenAI Python SDK** — GPT-4.1 integration
- **Google Gemini SDK** — Gemini 2.5 Flash integration
- **Python asyncio** — Full real-time orchestration of asynchronous battles
- **InquirerPy** — Interactive terminal interface for human-controlled play
- **Full Turn-by-Turn Logging** — Capturing every model prompt, game state, and tactical reasoning per turn

---

## Watch The Battles

### Battle 1 — Claude 4 vs Claude 3.7
Claude 4 demonstrated stronger predictive play, better setup timing, and superior awareness of win conditions.

**Video Recording:** _(Insert Video Here)_

---

## Setup: What The Models See Each Turn

### Full Battle State Provided:
- Weather, terrain, field hazards
- Current active Pokémon stats, moves, status, and boosts
- Opponent’s active Pokémon stats and status
- Team status (alive vs fainted)
- Last 10 turns of full battle history

### Decision Pipeline:
- Each model receives an identical natural language prompt describing full battle state
- Models respond with one action: **Use <move>** or **Switch to <Pokémon>**
- Each response includes one-sentence tactical reasoning
- If response is invalid, system defaults to random valid move
- Full logs record both prompt and model outputs for analysis

---

### Battle 2 — Claude 4 vs GPT-4.1
GPT-4.1 produced reasonable defensive play but struggled to handle multi-turn threats and shifting offensive momentum. Claude 4 steadily capitalized on every safe setup window.

**Video Recording:** _([Claude 4 vs GPT-4.1](https://youtu.be/h8rFj9WjwCU))_

---

### Battle 3 — Claude 4 vs Gemini 2.5 Flash (non-thinking)
Gemini 2.5 Flash showed quick reactions but often failed to escalate threats. Its switching logic frequently left it vulnerable against Claude 4’s highly coordinated stat-boosting sweepers.

**Video Recording:** _([Claude 4 vs Gemini 2.5 Flash (non-thinking)](https://youtu.be/P1VVkIv4HF0))_

---

## Deep Analysis: Why Claude 4 Emerged Supreme

### Exceptional Setup Timing
- Claude 4 expertly identified windows for stat boosts (Calm Mind, Nasty Plot, Quiver Dance) and sequenced them to maximum effect.
- It recognized when threats were temporarily neutralized and used those moments to stack power.

### Accurate Type and Coverage Calculations
- Chose super-effective coverage consistently.
- Examples: Knock Off vs Dunsparce, Focus Blast vs Gyarados, Psyshock vs Poison types like Overqwil — all correctly leveraging weaknesses.

### Smart Risk Management
- When opponents were low HP, Claude consistently opted for guaranteed KO moves rather than unnecessary setups.
- Managed status effects well, choosing safe damage-over-time win conditions (e.g., Scald burns).

### Multi-Turn Sequencing
- Balanced boosting, healing, and attacking based on board state.
- Didn’t tunnel into greedy play — adapted fluidly between aggression and defense depending on momentum.

### Predictive Opponent Modeling
- Correctly read opponent archetypes: stallers vs sweepers vs hazard-setters.
- Knew when opponents were unlikely to threaten back immediately.

### Minimal Tactical Errors
- Claude 4 exhibited almost zero critical mistakes across multiple full-length battles.
- Parsing failures were rare and generally due to rigid output parsing, not model reasoning flaws.

---

## Full Comparative Breakdown

| Category | Claude 4 | GPT-4.1 | Gemini 2.5 Flash |
|----------|----------|---------|------------------|
| Setup Timing | ⭐⭐⭐⭐⭐ | ⭐⭐ | ⭐ |
| Threat Recognition | ⭐⭐⭐⭐⭐ | ⭐⭐ | ⭐ |
| Risk Management | ⭐⭐⭐⭐⭐ | ⭐⭐ | ⭐⭐ |
| Recovery Use | ⭐⭐⭐⭐ | ⭐ | ⭐ |
| Switching Logic | Precise | Excessive | Erratic |
| Endgame Sequencing | Masterful | Inconsistent | Incomplete |

---

## Key Takeaways

Claude 4 displayed agentic-level long-horizon decision-making:

- **Strategic setup play** (stat boosts, accurate hazard usage)
- **Midgame control** (safe recovery, sequencing of offense/defense)
- **Endgame management** (optimal KO paths, minimal unforced errors)
- **Flexible tactical adjustments** (never stuck in single-mode play)

GPT-4.1 and Gemini both demonstrated reasonable but reactive playstyles — defaulting to safer moves without aggressive escalation.

Claude 4 played like a **high Elo competitive battler** — a benchmark that strongly suggests true agentic multi-turn reasoning capabilities in complex, stochastic environments.

---

### Teaser: Human vs Claude 4 Showdown

After model-vs-model testing, I went head-to-head against Claude 4 myself to see who is better, here is the full battle:

**Video Recording:** _(Insert Video Here)_



### Teaser: Human vs Claude 4 — The Ultimate Challenge
After benchmarking model vs model, I entered the arena myself to face off against Claude 4 directly. Using the same fully interactive interface, I manually made tactical decisions while Claude 4 operated autonomously.

👉 Watch the full human vs AI battles unfold — can human intuition outperform an agentic LLM in live tactical combat?
**Video Recording:** _(Insert Video Here)_

