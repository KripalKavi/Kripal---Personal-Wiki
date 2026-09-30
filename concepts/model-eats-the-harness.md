---
title: "Model Eats the Harness"
type: concept
date_added: 2026-04-28
tags: [ai, product-strategy, product-development, frameworks, microsoft-relevant]
sources: ["Lenny's Podcast, Cat Wu episode, 2026; Lenny's Podcast, Boris Cherny episode, 2026"]
related: ["../concepts/right-amount-agi-pilled.md", "../concepts/bitter-lesson.md", "../concepts/latent-demand.md", "../concepts/harness-as-moat.md", "../podcasts/lenny-cat-wu-ai-native-pm.md", "../podcasts/lenny-claude-code-boris-cherny.md"]
---

# Model Eats the Harness

## Definition

As AI models improve, the scaffolding, prompting interventions, and compensatory features built to work around prior model weaknesses become unnecessary — and should be systematically removed. The model "eats" the harness over time.

Phrase attributed to Boris Cherny ("the model will eat your harness for breakfast"). The operational practice of systematically removing it was described in detail by Cat Wu.

---

## Why It Matters

Product teams building on AI models tend to accumulate scaffolding — system prompt sections, reminder loops, to-do list features, rigid workflow constraints, UI elements — that were added to compensate for specific model weaknesses. This creates two problems:

1. **Scaffolding designed for an older model may actively fight a newer model**, reducing performance. What was a net positive at T-6 months may be a net negative at T+0.

2. **Heavy harness obscures model capability**. You're measuring harness+model performance, not model performance. You can't see what the model has become capable of.

The right practice: treat each new model launch as an opportunity to audit and simplify — not just expand.

---

## Examples

### Claude Code to-do list (Cat Wu's canonical example)

**Why it was added**: Early models would abandon multi-step tasks midway — fix 5 of 20 call sites, then stop. The to-do list forced state maintenance. Engineers had to remind the model: "Did you finish everything on the to-do list? You can't stop until you're done."

**How it worked**: The to-do list as a tool gave the model a structured memory artifact to track remaining work. Combined with prompting pressure, it reliably got models to completion.

**With Opus 4+ models**: The model naturally maintains and executes to-do lists without prompting. The feature is now **cosmetic** (visible progress for users) rather than **functional** (required for model behavior).

**Lesson**: A feature that was essential became unnecessary. Failing to recognize this would leave a prompting burden and a false dependency in the product.

### System prompt audit practice (Anthropic)

On every Claude Code model launch, the team reads the entire system prompt and asks of each section: "Does the model still need this reminder?" Sections that once compensated for tendencies — forgetting steps, skipping UI verification, not checking subagent work — are removed when the new model handles them naturally.

This is the heuristic operationalized as a process.

### New capabilities unlocked by harness removal

Code review was built and tested multiple times with earlier models. Accuracy was never high enough to ship. With Opus 4.5/4.6 and Sonnet 4.6, it became reliable enough to require as a merge gate — simultaneously a code review feature launch and a harness removal event (the scaffolding compensating for poor accuracy could be retired). Prototyping ahead of model capability meant zero ramp time when the model caught up.

---

## The Process

**At each model upgrade:**

1. Read through your entire prompting stack / system prompt
2. For each section: "Is this patching a current model weakness, or is this genuinely improving experience?"
3. Remove the patches
4. Check what new capabilities the model now enables that prior accuracy prevented you from shipping
5. Update product design for the simplified model

**Building ahead**: Features that can't ship today because accuracy isn't high enough should still be prototyped. When the model improves, you have a working product surface to plug it into — not a roadmap item to start from scratch.

---

## PM Application

**For Copilot at Microsoft:**

1. **Audit the scaffolding on every model upgrade.** Every time a new model ships in Azure OpenAI, GitHub Copilot, or Copilot in M365, the right question is not just "what new capabilities does this unlock?" but "what existing scaffolding can we now remove?" Prompt engineering layers, orchestration rules, and compensatory UX elements designed for GPT-4-era weaknesses may create friction against GPT-4o or GPT-5's natural behavior.

2. **Distinguish cosmetic from functional scaffolding.** Some scaffolding improves user experience even when the model no longer needs it functionally (visible progress, status messages, confirmation UI). Keep that. Systematically retire the functional crutches.

3. **Build features that don't work yet.** For Copilot features where model accuracy isn't good enough to ship, build the product design anyway and keep it in private preview or internal dogfood. When the next model ships, you're ready to turn it on — not starting from scratch.

4. **Treat your prompt engineering as temporary.** Any section of a system prompt or orchestration rule that exists to compensate for a current model weakness should be tagged as "expected to remove in [timeframe]." This changes how you invest in it and makes the audit process easier.

---

## Sources

- [Lenny's Podcast — Cat Wu, AI-native PM](../podcasts/lenny-cat-wu-ai-native-pm.md) — Primary articulation; to-do list example; system prompt audit practice
- [Lenny's Podcast — Boris Cherny, Head of Claude Code](../podcasts/lenny-claude-code-boris-cherny.md) — "Don't box the model in"; scaffolding gains get wiped by next model

## Related

- [Right Amount of AGI-Pilled](../concepts/right-amount-agi-pilled.md) — Calibrating how much to build for current vs. future model; this concept is the corrective mechanism when you've over-built
- [The Bitter Lesson](../concepts/bitter-lesson.md) — General model always wins; scaffolding that fights this delays the inevitable
- [Latent Demand](../concepts/latent-demand.md) — Build for what the model naturally wants to do, not against it
- [Harness as Moat](../concepts/harness-as-moat.md) — The external counterpart at the workspace layer. *This* concept is about the internal compensatory harness shrinking; *that* one is about the external workspace harness compounding as a moat. Both are true; they operate at different layers.
