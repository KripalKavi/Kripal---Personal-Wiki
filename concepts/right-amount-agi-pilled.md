---
title: "Right Amount of AGI-Pilled"
type: concept
date_added: 2026-04-28
tags: [ai, product-strategy, frameworks, microsoft-relevant]
sources: ["Lenny's Podcast, Cat Wu episode, 2026"]
related: ["../concepts/model-eats-the-harness.md", "../concepts/latent-demand.md", "../concepts/bitter-lesson.md", "../podcasts/lenny-cat-wu-ai-native-pm.md", "../podcasts/lenny-claude-code-boris-cherny.md", "../entities/cat-wu.md"]
---

# Right Amount of AGI-Pilled

## Definition

The challenge of calibrating AI product design to the capability of current models rather than hypothetical superintelligence. Being "AGI-pilled" means believing that models will eventually be so capable that most product complexity becomes unnecessary. The tension: that future is real, but acting as if it's already arrived produces bad products today.

> "It is very hard to be the right amount of AGI-pilled. It's very easy to build the product for the super AGI strong model. The hard thing is figuring out for the current model, how do you elicit the maximum capability?"
> — Cat Wu, Head of Product, Claude Code & Cowork, Anthropic

---

## Why It Matters

The supermodel case is trivially easy to design for: if the AI can do anything, you just need a text box. The model adds its own tools, knows when to ask for clarification, handles ambiguity — no scaffolding required. This is easy to envision, easy to build toward, and feels like "thinking big."

But that's not the model you have. Most product value comes from bridging the gap between today's model and that vision in a way that creates value now. This requires:

- Deeply understanding current model failure modes
- Designing product surfaces that guide users to the golden path (model strengths)
- Patching model weaknesses in the product layer (without waiting for the next model)
- Constantly recalibrating as models improve

Vision is not the hard part. Execution on current capability is.

---

## The Spectrum

**Too AGI-pilled (underbuilding for today)**: Shipping a simple prompt interface and assuming users will figure it out. Users hit walls repeatedly because the product doesn't compensate for known model weaknesses. Low activation, poor retention.

**Not AGI-pilled enough (overbuilding for today)**: Adding elaborate scaffolding, rigid workflows, and compensatory UI components that the next model will make obsolete — and that may actively constrain performance. See [Model Eats the Harness](../concepts/model-eats-the-harness.md).

**Calibrated correctly**: Building features that solve today's real failure modes, minimally enough that the next model can absorb or replace the scaffolding. The Claude Code to-do list was correct scaffolding for its era; removing it when models no longer needed it was equally correct.

---

## Relationship to Adjacent Concepts

**Tension with "Build for the model 6 months out" (Boris Cherny)**: Boris's advice is to design for future model capability — accept poor PMF now for strong PMF at inflection. Cat Wu's concept is complementary, not contradictory: design the *product surface* for future capability, but design the *scaffolding and golden paths* for today's model. Don't over-invest in compensatory scaffolding, but do invest in eliciting maximum current performance.

**Enables [Model Eats the Harness](../concepts/model-eats-the-harness.md)**: Getting the calibration right requires knowing which scaffolding is permanent product design vs. temporary model compensation. The latter should be systematically removed as models improve.

**Grounded by [Latent Demand](../concepts/latent-demand.md)**: Observing what users are currently able and unable to accomplish with the model is the empirical input for calibration. Users' workarounds and failures are a map of where current model capability falls short.

---

## PM Application

**For Copilot product teams at Microsoft:**

1. **Audit the "waiting for the next model" backlog**: Any feature decision deferred with "the model will be smarter soon" is AGI-pilling. Some deferral is right; most isn't. For each deferred item, ask: what would it take to make this work *today*? Sometimes the answer is golden-path design, not a better model.

2. **Invest in golden-path design**: The question "what sequence of interactions reliably produces value from today's model?" is the hardest product question and the most valuable thing to answer. Most Copilot features under-invest here relative to feature breadth.

3. **Don't over-scaffolded against AGI**: When the next generation model ships, scaffolding that was designed for GPT-4 may fight against what GPT-5 naturally does well. Build the minimum scaffolding needed to solve today's failure modes — no more.

4. **Treat this as a moving calibration**: With model improvements every few months, the right product design is not stable. Build re-evaluation of your calibration into model upgrade cycles, not just "what new things can we enable?"

---

## Sources

- [Lenny's Podcast — Cat Wu, AI-native PM](../podcasts/lenny-cat-wu-ai-native-pm.md) — Primary articulation; coined the term
- [Lenny's Podcast — Boris Cherny, Head of Claude Code](../podcasts/lenny-claude-code-boris-cherny.md) — Complementary principle: "Build for the model 6 months out"
- [Lenny's Podcast — Max Schoening, Notion](../podcasts/lenny-max-schoening-agency-over-skills.md) — Related claim: **intelligence has a "retina display" ceiling.** For most knowledge work, model intelligence saturates; once past saturation, speed of inference and modality matter more than raw IQ. Implication: stop designing only for the next supermodel; design also for cheap-fast-local. *"Society is largely not capped by intelligence."*

## Related

- [Model Eats the Harness](../concepts/model-eats-the-harness.md) — The mechanism for correcting when you've over-built scaffolding
- [Latent Demand](../concepts/latent-demand.md) — What users can't do today = map of current model limits = calibration input
- [The Bitter Lesson](../concepts/bitter-lesson.md) — General model always wins long-term; this concept governs the *short-term* product layer
