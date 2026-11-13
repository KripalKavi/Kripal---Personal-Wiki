---
title: "The Bitter Lesson"
type: concept
date_added: 2026-04-19
tags: [ai, product-strategy, frameworks, microsoft-relevant]
sources: ["https://www.lennysnewsletter.com/p/head-of-claude-code-what-happens"]
related: ["../podcasts/lenny-claude-code-boris-cherny.md", "../entities/boris-cherny.md"]
---

# The Bitter Lesson

---

## Definition

A foundational principle in AI from Rich Sutton (2019): **the more general approach will always outperform the more specific approach over the long run**.

The "bitter" part: researchers and engineers who invest heavily in human-crafted knowledge representations, domain-specific rules, and specialized systems repeatedly get beaten by simpler, more general approaches with more compute and data. The lesson is bitter because the specialized work feels sophisticated and the general approach feels lazy — but the general approach wins.

Boris Cherny cites this as a core operating principle for the Claude Code team.

---

## Why It Matters

The natural instinct when building on AI models is to add structure: fine-tune the model for your domain, add scaffolding to constrain its behavior, layer in custom logic to handle edge cases. Each of these feels like it's making the system better. Often it does — temporarily. But when the next generation of the base model ships, those customizations frequently lose their advantage or become liabilities.

The Bitter Lesson predicts this: general improvement compounds faster than specific optimization. Betting on the general model means you get the next model's improvements for free. Betting on customization means you have to redo the work with each new model.

---

## Corollaries for AI Product Building

Boris applies the Bitter Lesson broadly:

1. **Don't fine-tune when you can use the base model**: Custom fine-tuning is expensive to maintain, and next-generation base models often exceed what fine-tuning achieved. Reserve fine-tuning for cases where the base model genuinely can't do the job.

2. **Don't use smaller models to save costs — it often costs more**: Using Sonnet instead of Opus to save on token costs often backfires — the smaller model makes more mistakes, requires more correction, and uses more tokens total. The capable model does it right in fewer turns.

3. **Don't build rigid scaffolding — it gets wiped out by the next model**: Step-by-step orchestration systems that constrain how the model operates may improve performance 10–20% today. But the next model generation often makes those gains irrelevant while the scaffolding adds maintenance overhead.

4. **Wait for the next model, not the next customization**: When a use case doesn't work well today, the default should be "is this a model capability problem?" If yes, the better bet is often to wait for the next model release than to engineer around the limitation.

---

## The Tension

The Bitter Lesson creates a real tension for product teams:
- You can't just wait for the next model — you have to ship something
- Some customization is necessary and appropriate (system prompts, tool design, output formatting)
- The lesson is about *where to place your bets*, not about doing nothing

The practical application: be very skeptical of investments in model customization that have to be redone with each model generation. Prefer architectural choices that are model-agnostic and that get better automatically as base models improve.

---

## PM Application

For a Senior Director of PM at Microsoft:

1. **Azure AI / Copilot architecture decisions**: When engineering teams propose fine-tuning a model for a specific Copilot vertical (legal, healthcare, finance), apply the Bitter Lesson test: is this a capability gap that the next base model will likely close? If yes, the fine-tuning investment has a short shelf life. This should be a factor in build/wait decisions.

2. **Evaluate scaffolding investments skeptically**: When teams propose complex prompt orchestration systems or multi-step LLM workflows, ask: what's the maintenance burden when GPT-5 / Claude 4 ships? If the scaffolding needs to be rebuilt, that cost should factor into the decision.

3. **Token cost optimization timing**: Follow Boris's principle — don't optimize costs during the discovery phase. The Bitter Lesson version: don't reduce model size prematurely. Get to product-market fit on the best available model, then optimize. Premature cost optimization reduces capability before you know what capability you need.

4. **Model upgrade strategy**: Design Copilot features to be model-agnostic where possible. Every Microsoft AI feature that's tightly coupled to a specific model version has an implicit expiration date and an upgrade cost. Prefer designs that benefit automatically from model improvements.

---

## Sources

- [Head of Claude Code: What Happens After Coding Is Solved](../podcasts/lenny-claude-code-boris-cherny.md) (Boris Cherny, 2026-02-19)
- Original: Rich Sutton, "The Bitter Lesson" (blog post, 2019)
