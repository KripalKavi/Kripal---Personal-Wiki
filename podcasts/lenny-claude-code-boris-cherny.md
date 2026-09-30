---
title: "Head of Claude Code: What Happens After Coding Is Solved"
type: podcast
date_added: 2026-04-19
tags: [ai, coding, product-development, anthropic, latent-demand, frameworks, microsoft-relevant]
sources: ["https://www.lennysnewsletter.com/p/head-of-claude-code-what-happens"]
related: ["../entities/boris-cherny.md", "../entities/anthropic.md", "../concepts/ai-product-activation.md", "../concepts/latent-demand.md", "../concepts/bitter-lesson.md"]
---

# Head of Claude Code: What Happens After Coding Is Solved

**Show**: Lenny's Podcast
**Guest**: [Boris Cherny](../entities/boris-cherny.md), Creator and Head of Claude Code, Anthropic
**Host**: Lenny Rachitsky
**Published**: 2026-02-19
**Source**: https://www.lennysnewsletter.com/p/head-of-claude-code-what-happens

---

## Summary

Boris Cherny, who built Claude Code from a one-person terminal prototype, makes the case that coding is effectively solved — and explores what comes next. The episode is one of the richest available sources on how to build AI products, covering latent demand, model-forward product design, the Bitter Lesson, and what it means for organizational structure when AI writes all the code.

---

## Key Takeaways

### "Coding is virtually solved"
- Boris's 100% of code has been written by Claude Code since November 2025; he ships 10–30 pull requests per day
- Claude Code accounts for 4% of all public GitHub commits (private repos likely higher); predicted to hit 20% by end of 2026
- Spotify's best developers haven't written a line of code manually since December 2025
- Growth rate is *accelerating*, not just growing — "any metric you look at, it keeps going up faster and faster"
- The trajectory to 100% was foreseeable: Boris traced the exponential in May 2025 and the room gasped at his prediction; by November it was true for him personally

### Latent demand — the single most important product principle
Boris's most detailed framework, with two dimensions:

**Traditional latent demand**: Find where users are already abusing your product to do something it wasn't designed for. That's your next product.
- Facebook Marketplace came from observing 40% of Facebook Group posts were buying/selling — people were hacking Groups to trade
- Facebook Dating came from observing 60% of profile views were people of opposite gender who weren't friends — people were using Facebook to scope out potential partners
- Cowork came from observing non-technical users running Claude Code in a terminal to: grow tomato plants, analyze their genome, recover corrupted wedding photos, analyze MRIs — none of these are coding tasks

**Modern latent demand — applied to the model**: Not just what users are doing, but what the model is *trying* to do.
- Traditional AI product design: put the model in a box, define its role, give it a specific function
- Claude Code inverted this: "the product IS the model" — minimal scaffolding, give it tools, let it decide which tools to use and in what order
- In research terms: "be on distribution" — don't fight what the model naturally wants to do, find out what that is and build around it
- This is latent demand applied one layer deeper: the model's own behavior reveals product direction

### Don't box the model in
- Most teams impose rigid workflows on LLMs: "do step 1, then step 2, then step 3"
- Scaffolding can improve performance ~10–20% — but those gains get wiped out with the next model release
- Better approach: give the model a goal and tools, let it figure out the path
- Boris's example: a senior engineer was manually debugging a memory leak the traditional way (heap snapshots, debugger). A newer engineer just said "Claude, there's a leak, figure it out." Claude wrote its own analysis tool, found the bug, opened a PR — faster than the senior engineer.
- Implication: the model you built around six months ago is no longer the model you have

### The Bitter Lesson — bet on the general model
- A foundational principle for the Claude Code team, from Rich Sutton's essay
- Core insight: the more general model will always outperform the more specific model over the long run
- Corollaries:
  - Don't fine-tune when you can use the base model
  - Don't build elaborate scaffolding — wait for the next model
  - Don't use smaller cheaper models — Opus often uses *fewer* tokens total because it makes fewer mistakes and needs less correction; false economy to use Sonnet
- "Always bet on the more general model"

### Build for the model six months from now, not today
- Claude Code had poor product-market fit for the first six months — the model wasn't capable enough
- The bet: build for what the model *will* be able to do, not what it can do today
- When Opus 4 shipped (first ASL3 model, May 2025), everything inflected — users flooded in because the product was already designed for a capable model
- Advice for startups: "It's going to be uncomfortable because your PMF won't be very good for the first six months. But when that model comes out you'll hit the ground running."
- Boris had visibility into model trajectories; but public signals also work — if the model is "almost good enough," trace the exponential

### Under-resourcing as a forcing function
- Counterintuitive principle: put one engineer on a project, and they're forced to Claude-ify everything
- Intrinsic motivation (wanting to ship) + Claude + no choice = maximum AI leverage
- "Give engineers as many tokens as they want at the start. Don't optimize costs until after you've found what works."
- Some Anthropic engineers now spending $100K+/month in tokens — this is a *perk* some companies are starting to offer
- The optimization point: once you've proven the idea, then figure out whether Haiku or Sonnet can do it instead of Opus

### "The title software engineer is going to start to go away"
- By end of 2026: "everyone is going to be a product manager, and everyone codes"
- The replacement title: **builder** — someone who ships, regardless of their background
- On the Claude Code team: PM codes, engineering manager codes, designer codes, finance person codes, data scientist codes
- Already seeing 50% overlap in what PMs, designers, and engineers do day-to-day
- Boris's advice to survive: "Be a generalist. Cross disciplines. An engineer with great design sense, or with strong business judgment, or who loves talking to users — those are the people who will be rewarded."

### Three-layer safety model (Anthropic's framework)
1. **Alignment / mechanistic interpretability**: Study the neurons — what concepts does each encode? (Chris Olah's work at Anthropic; they can now detect things like "deception neuron activation")
2. **Evals**: Laboratory setting — synthetic situations to test whether the model behaves correctly
3. **Real-world behavior**: How the model actually behaves in production — the hardest to fake; released Claude Code early specifically to study this at scale
- Important: a model can look great on layers 1 and 2 but behave unexpectedly in layer 3
- This connects directly to [AI Evals](../concepts/ai-evals.md) — evals are layer 2, but you need all three

### Anthropic's intentional design path: coding → tool use → computer use
- This has been the explicit model development roadmap since founding — not accidental
- Each stage teaches the model something needed for safe AGI: coding = precise reasoning; tool use = acting in the world; computer use = interacting with unstructured environments
- Every product decision maps to safety research needs, not just revenue

### Cowork built in 10 days with Claude Code
- Observed non-technical people hacking Claude Code for non-coding tasks → obvious latent demand
- Team explored options for months, then someone said "what if we just put Claude Code in the desktop app?"
- Entire virtual machine + security guardrails: written by Claude Code
- Launched rough, on purpose: "We have to release things a little bit earlier than we think so we can get the feedback"
- Cowork grew faster in early days than Claude Code did — lesson: when you nail latent demand, adoption is immediate

---

## Notable Quotes

> "Latent demand is the single most important principle in product." — Boris Cherny

> "By the end of the year, everyone is going to be a product manager, and everyone codes. The title software engineer is going to start to go away. It's just going to be replaced by builder."

> "Coding is virtually solved."

> "I have never enjoyed coding as much as I do today, because I don't have to deal with all the minutia."

> "Don't try to box the model in. Give it the tools. Give it a goal. Let it figure it out."

> "Build for the model six months from now, not for the model of today."

> "Start by just giving engineers as many tokens as possible." 

> "The fun part is figuring out what to build. Talking to users. Thinking about big systems. Collaborating. That's what I get to do more of now." (on coding being solved)

---

## Frameworks Introduced

- **[Latent Demand](../concepts/latent-demand.md)** — Find what users are already doing outside your product's designed use; that's your next product. Modern extension: find what the model is trying to do.
- **[The Bitter Lesson](../concepts/bitter-lesson.md)** — General models always outperform specific ones over the long run. Bet on generality, not customization.
- **Build for the model 6 months out** — Design product for model capability that doesn't exist yet; accept poor PMF now for strong PMF at the inflection
- **Don't box the model in** — Give goal + tools, not step-by-step workflows
- **Three-layer safety model** — Alignment → Evals → Real-world behavior (all three required)

---

## PM Relevance

1. **Latent demand is the highest-ROI product discovery method for AI**: Don't specify what AI features to build — watch what people are already doing with your AI product that you didn't design for. For Copilot in M365: What are users doing in Copilot that the product wasn't explicitly designed for? Those behaviors point to the next product surface. The modern extension: what is Copilot naturally trying to do when given latitude? That's your roadmap signal.

2. **GitHub Copilot competitive intelligence — the direct competitor**: Claude Code went from terminal prototype to 4% of GitHub commits in one year, with a growth rate that is *still accelerating*. The product philosophy that drove this (latent demand, minimal scaffolding, build for the next model) is the exact playbook Microsoft needs to understand and respond to. The "builder" framing that replaces "software engineer" is the competitive vision Boris is executing against.

3. **"Builder" replaces "software engineer" — org design implications**: Boris is explicit that by end of 2026, the PM/design/engineering distinction will blur significantly. A Senior Director at Microsoft should be watching for this: what does a Microsoft product team look like when all team members can ship code? Headcount strategy, role definitions, and career ladders built around the old model are already becoming obsolete.

4. **Don't box Copilot in**: When building Copilot features, the instinct is to define tightly what the AI should do in a given scenario. Boris's data shows this is the wrong approach — give the model tools and a goal. This applies to how Microsoft's prompt engineering and orchestration work is done: minimize the scaffolding, let the model navigate.

5. **The Bitter Lesson for Azure AI strategy**: Don't fine-tune when you can use a better base model. This is directly actionable for teams at Microsoft building on top of Azure OpenAI — the investment in custom fine-tuning often gets wiped out by the next model generation. Bet on the general model.

6. **Unlimited tokens as a team productivity principle**: Boris's advice is explicit — don't optimize token costs during the discovery phase. Give teams building Copilot features unlimited or very generous AI budgets. The cost of token constraints is invisible (ideas not tried, feedback loops not closed) but real.

7. **"Build for the model 6 months out" for Copilot roadmap**: If you build Copilot features for the model that exists today, they'll feel underwhelming at launch. Build for the model capabilities that are coming — accept that the feature will look rough initially. This is a planning philosophy change.

8. **Three-layer safety: evals are necessary but not sufficient**: The AI Evals framework from Hamel/Shreya covers layer 2. Boris's framing adds that layer 3 (real-world behavior) is what you can't study in a lab. Copilot features need all three: alignment/safety review, eval suites, and real-world monitoring of actual user behavior.

---

## Books Recommended

From the lightning round ("two or three books you recommend most"):

- [Functional Programming in Scala](../books/chiusano-bjarnason-functional-programming-scala.md) — Chiusano & Bjarnason (2014). "The single best technical book I have ever read." The thinking-in-types mindset Boris can't stop applying, even now that AI writes all his code.
- [Accelerando](../books/stross-accelerando.md) — Charles Stross (2005). "Captures the essence of this moment more than any other book." Three-generation singularity novel whose narrative pace mirrors technological acceleration.
- [The Wandering Earth](../books/liu-cixin-wandering-earth.md) — Liu Cixin (short stories). Preferred over *Three Body Problem*. "Very different perspective than Western sci-fi." Civilizational scale, collective actors, long time horizons.

---

## Entities Mentioned

- [Boris Cherny](../entities/boris-cherny.md) — Creator of Claude Code, Anthropic
- [Anthropic](../entities/anthropic.md) — Developer of Claude and Claude Code

## Concepts Introduced

- [Latent Demand](../concepts/latent-demand.md) — Find what users are doing outside product design; that's your next product
- [The Bitter Lesson](../concepts/bitter-lesson.md) — General models always outperform specific ones long-term
- [AI Product Activation](../concepts/ai-product-activation.md) — Activation as the key challenge once coding friction is removed
- [AI Evals](../concepts/ai-evals.md) — Evals are layer 2 of a three-layer safety and quality model
