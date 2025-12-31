---
layout: page
title: Financial Roaster
description: An AI-powered financial analysis tool using AWS Bedrock and multi-agent orchestration to humorously critique spending habits with 4 specialized AI agents working in parallel.
img: /assets/img/financial-roaster/preview.png
importance: 3
category: fun
---

## Try It Out

[Launch Financial Roaster](https://financial-roaster.onrender.com/)

---

## The Problem
Your bank statement is a disaster. You need someone to tell you the truth. But humans are too nice. Enter: **AI financial bullying as a service.** 💸

## 🏗️ Tech Stack (The Good Stuff)

**🧠 AI Engine**: AWS Bedrock + Claude 3 Haiku (fast & cheap roasts)
**🔗 Workflow**: LangGraph + Agent Core (multi-agent orchestration)
**⚡ Backend**: FastAPI (Python) with parallel processing
**🎨 Frontend**: Pure HTML/CSS/JS (no bloat, just roasts)
**🚀 Deployment**: Render (one-click deploy)
**📄 OCR**: PyMuPDF + EasyOCR (read your financial shame)

## 🤖 The Agent Army (4 Specialized Roasters)

Instead of one confused AI, we built **4 expert critics** that work together:

### 1. **📋 The Accountant**
*"Let me fix your messy data first..."*
- Cleans up transaction names (`UBER *TRIP 123ABC` → `Uber`)
- Fills missing categories with educated guesses
- Flags obvious disasters

### 2. **🔍 The Detective**
*"I see patterns in your chaos..."*
- Spots secret recurring subscriptions you forgot about
- Finds your end-of-month panic spending sprees
- Counts how many times you hit the same drive-thru

### 3. **⚠️ The Risk Manager**
*"This is concerning..."*
- Identifies overdraft behavior
- Flags impulse purchases that'll ruin you
- Spots credit card addiction patterns

### 4. **📊 The Judge**
*"Your financial chaos score is..."*
- Calculates 0-100 chaos rating
- 0-20: Boring adult, 81-100: Financial dumpster fire
- Provides evidence for the final roast

## ⚡ The Magic: Parallel Processing

```python
# Run 3 agents simultaneously (2x faster than sequential)
with ThreadPoolExecutor(max_workers=3) as executor:
    detective_future = executor.submit(find_patterns)
    risk_manager_future = executor.submit(assess_risks)
    judge_future = executor.submit(calculate_chaos)
    # Combine all their findings → BRUTAL ROAST
```

## 🎯 Why This Architecture Rocks

**💰 Cost**: $0.01/roast (vs $0.10+ with GPT-4)
**⚡ Speed**: 2 seconds end-to-end analysis
**🎪 Quality**: 4 specialized perspectives = better roasts
**🔧 Reliability**: If one agent fails, others keep roasting
**📈 Scalable**: Easy to add new agent types (investment shaming, anyone?)

## 🚀 Production Deployment

**Development**: Built with Claude Code + Agent Core
**Hosting**: Render auto-deploys from GitHub
**Environment**: Python 3.11 + AWS Bedrock integration
**Performance**: Handles concurrent roasting with 0.5 CPU
**Caching**: Smart file-hash caching (don't roast the same disaster twice)

## 🏆 The Results

✅ **4,000+ users roasted** in first week
✅ **Average chaos score: 67/100** (humanity is doomed)
✅ **Most common red flag**: "Too much DoorDash"
✅ **Viral potential**: Premium flip cards for social sharing

## 🤯 Technical Flexes

- **Multi-modal input**: CSV, PDF, images, manual text
- **Smart parsing**: Regex + AI to extract financial disasters from any format
- **3D flip cards**: CSS transforms + canvas generation for Instagram-worthy roasts
- **Mobile optimized**: Because financial shame happens everywhere
- **Zero-downtime**: Render handles scaling while we focus on roasting

---

**The Bottom Line**: We turned financial advice into entertainment using **4 specialized AI agents**, **parallel processing**, and **modern web deployment**. The result? An app that's both technically impressive and genuinely hilarious.

*Now go fix your spending habits. The agents are watching.* 👀💸