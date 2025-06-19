---
layout: page
title: "Large Language Models Pokémon Battle Arena"
description: "Claude 4 vs GPT-4.1 vs Gemini 2.5 Flash vs Human in AI Pokémon Battle"
img: "/assets/img/Pokemon/Pokemon_Logo.png"
importance: 3
category: fun
---

# Introduction

This is a fun experiment to battle-test the limits of today’s large language models — not with dry benchmarks, but by throwing them into a Pokémon arena.

Each model takes full control of its team, making real-time decisions as if it were a competitive Pokémon trainer. To push the models’ reasoning skills, I selected “non-thinking” frontier models — meaning they must rely entirely on their base reasoning without chain-of-thought scaffolding.

In this arena, we can observe how well leading LLMs handle multi-turn strategy, risk management, adaptive planning, and real-time tactical combat — all while trying to become Pokémon champion.

## Competitors

* **Claude 3.7** (Anthropic)
* **Claude 4** (Anthropic)
* **GPT-4.1** (OpenAI)
* **Gemini 2.5 Flash** (Google)
* **Human** (myself)

All battles were conducted using Pokémon Showdown’s `gen9randombattle` format, ensuring randomized but balanced teams. Also all model used the exactly same prompt, therefore the difference should lies in the internal decision making of each LLM and its reasoning ability to make the right long-term decision.

# Setup: How LLMs Think Like Pokémon Trainers

Once connected to the battle environment, each language model steps into the role of a fully autonomous Pokémon trainer. But what makes this interesting isn’t just the mechanics — it’s how each LLM processes complex battle state information to make decisions under uncertainty.

At every turn, the model receives a full natural language summary of the current battle state, including:

* Active Pokémon on both sides, with full stats, typing, move sets, current boosts, and status conditions.
* Remaining team members (alive vs fainted).
* Field hazards (spikes, stealth rock, terrain effects, weather).
* Recent turn history (actions taken over the last 3 turns, to mimic human-like memory).

# Battle Log

## Winner: Claude 4

I simulated 10 battles between Claude 3.7 and Claude 4, the results are Claude 4 was able to win ~80% of the time.

[![Claude 4 vs Claude 3.7](/assets/img/pokemon_ai_battle/claude4_vs_claude37_thumb.png)](https://youtu.be/YOUR_VIDEO_LINK)

In head-to-head matchups:

- 3 battles between Claude 4 and GPT-4.1 — Claude 4 won all of them.
[Cladue 4 vs GPT 4.1](https://youtu.be/h8rFj9WjwCU)

- 3 battles between Claude 4 and Gemini 2.5 Flash — Claude 4 won all of them.
[Cladue 4 vs gEMINI 2.5 Flash](https://youtu.be/P1VVkIv4HF0)


## 2nd Place: Claude 3.7

Claude 3.7 showed very strong base reasoning and tactical awareness, consistently outperforming GPT-4.1 and Gemini 2.5 Flash in most simulations. While slightly less refined in long-term sequencing compared to Claude 4, it still demonstrated high-level multi-turn planning.

---

# Full Comparative Breakdown

| Skill Category     | Claude 4  | Claude 3.7  | GPT-4.1      | Gemini 2.5 Flash |
| ------------------ | --------- | ------------ | ------------ | ---------------- |
| **Opening Strategy (Early Game Setup)** | ⭐⭐⭐⭐ | ⭐⭐⭐⭐  | ⭐⭐⭐    | ⭐⭐⭐ |
| **Threat Recognition (Identifying Dangers)** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐  | ⭐⭐    | ⭐⭐ |
| **Risk Management (Balancing Safety vs Aggression)** | ⭐⭐⭐⭐ | ⭐⭐⭐⭐  | ⭐⭐⭐  | ⭐⭐ |
| **Recovery Usage (Healing Correctly)** | ⭐⭐⭐ | ⭐⭐⭐  | ⭐    | ⭐ |
| **Switching Logic (Choosing Correct Pokémon Swap)** | Precise | Good | Overreactive | Erratic |
| **Endgame Planning (Finishing the Match Efficiently)** | Masterful | Strong | Inconsistent | Incomplete |

---

# Key Takeaways

Claude 4 exhibited advanced multi-turn, long-horizon tactical reasoning:

* Strategic setup and hazard management
* Balanced midgame control and recovery
* Optimal endgame KO pathing
* Flexible adaptation to evolving game state

**Claude 3.7** showed reliable turn-by-turn reasoning, often making solid risk-adjusted decisions, but lacked some of the deeper foresight Claude 4 displayed during complicated endgame situations.

GPT-4.1 and Gemini displayed safer, reactive playstyles with limited proactive escalation.

Claude 4 operated with **high Elo competitive skill**, suggesting genuine agentic multi-turn reasoning capabilities even in stochastic, open-ended environments.

---

# Teaser: Human vs Claude 4

To further test Claude 4's capabilities, I entered the arena directly, making live tactical decisions while Claude 4 operated autonomously.
[![Claude 4 vs Myself!](/assets/img/pokemon_ai_battle/claude4_vs_claude37_thumb.png)](https://youtu.be/iB_NjlXiDKQ)

