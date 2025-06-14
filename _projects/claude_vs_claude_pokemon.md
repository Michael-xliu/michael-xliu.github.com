---
layout: page
title:  Pokémon AI Battle
description: Claude 3.7 vs Claude 4.0 in a Strategic Pokémon Showdown
img: /assets/img/Pokemon/Pokemon Logo.png
importance: 3
category: fun
---


## Introduction

In this project, I built a fully automated Pokémon battle system using two Claude models from Anthropic—Claude 3.7 and the latest Claude 4.0—pitted against each other in real-time via a local Pokémon Showdown server.

The objective? See how each LLM reasons and strategizes when given full battle information—testing their decision-making capabilities turn by turn.

## Watch the Battle

D:\SMU DS\Michael'swebsite\michael-xliu.github.com\assets\video\Claude 4 vs 3.7.mp4

<video controls width="800" poster="/assets/img/Pokemon/Screenshot.png">
  <source src="/assets/video/Claude 4 vs 3.7.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

## Setup Overview

The project leverages the `poke-env` Python framework to simulate turn-based Pokémon battles. Each Claude model acts as a `Player`, making decisions based only on the current game state.

### Technical Stack

- **poke-env**: Python environment for simulating Showdown battles
- **Anthropic Claude**: Accessed via Amazon Bedrock API
- **Python asyncio**: For managing concurrent battles
- **Custom Battle Player Class**: Wrapped logic for decision-making using Claude

## How Claude Makes Decisions

For each turn, Claude is provided a prompt that includes:

- Current turn number and weather conditions
- Active and opposing Pokémon stats, types, boosts, and status
- Full move sets for the active Pokémon
- Remaining team members and their condition
- Side hazards and terrain

Claude is then instructed to:

- Choose one action: either `Use <move>` or `Switch to <Pokémon>`
- Provide a one-sentence explanation of the tactic

Here's an example of Claude's output:

```
[Turn 2] [Claude 3.7] is thinking...
[Claude 3.7] replied: Switch to Rotom-Heat
Toxapex is at critically low health and vulnerable to Gardevoir's Psychic attacks.

[Turn 3] [Claude 4] is thinking...
[Claude 4] replied: Use Moonblast
A STAB Moonblast threatens most of the opponent's team and ensures pressure.
```

## Battle Format & Teams

- **Format**: `gen9ou` (OU = OverUsed tier — popular competitive Pokémon)
- **Teams**: Fixed 6-member competitive teams with balanced offense and defense
- **Movesets**: Standard Smogon-style sets with diverse strategies like stall, setup, or sweep

## Results: Claude 4 Dominates

After running multiple 1v1 matches:

- Claude 4.0 **won almost every battle**
- It made more reliable tactical decisions and switch predictions
- It adapted better when low-health or cornered

## Observations

- Claude 3.7 sometimes overcommitted to setup moves
- Claude 4.0 showed better threat assessment and win-con awareness
- The slow-down between turns improved readability and animation sync


## Future Work

- Add expressive personalities (e.g., aggressive vs defensive Claude)
- Try formats like `gen9randombattle` or doubles
- Benchmark against GPT-4 or Gemini Models

## Code & Setup

The full implementation includes Claude model prompting, real-time game rendering, and terminal-based strategy logs.

[View on GitHub](https://github.com/yourusername/claude-pokemon-battle)

If you’re interested in LLMs applied to games or autonomous agent reasoning—this was an incredibly fun and insightful experiment!

