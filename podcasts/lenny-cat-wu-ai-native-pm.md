---
title: "How to Be a Great PM for AI Native Products"
type: podcast
date_added: 2026-04-28
tags: [ai, product-strategy, product-development, anthropic, frameworks, velocity, microsoft-relevant]
sources: ["Lenny's Podcast, Cat Wu episode, 2026 (transcript)"]
related: ["../entities/cat-wu.md", "../entities/anthropic.md", "../entities/boris-cherny.md", "../podcasts/lenny-anthropic-growth-amol-avasare.md", "../podcasts/lenny-claude-code-boris-cherny.md", "../concepts/right-amount-agi-pilled.md", "../concepts/model-eats-the-harness.md", "../concepts/ai-evals.md", "../concepts/latent-demand.md"]
---

# How to Be a Great PM for AI Native Products

**Show**: Lenny's Podcast
**Guest**: [Cat Wu](../entities/cat-wu.md), Head of Product for Claude Code and Cowork, Anthropic
**Host**: Lenny Rachitsky
**Published**: 2026 (transcript ingested 2026-04-28)
**Source**: Transcript (direct)

---

## Summary

Cat Wu, who runs product for Claude Code and Cowork — the two Anthropic products most directly redefining how software is built — lays out a comprehensive account of what AI-native PM looks like in practice. The episode covers how to ship at weekly velocity, how to calibrate product vision to current model capability, why product taste has become the scarce skill, and how Anthropic structured its process to ship features in a day. Dense with deployable frameworks.

---

## Key Takeaways

### The PM role has fundamentally shifted to velocity

Before AI, technology shifts were slow enough to plan on 6–12 month horizons. Coordination with partner teams mattered because code was expensive. Now:

- Feature timelines have collapsed from 6 months → 1 month → 1 week → 1 day
- The PM's coordination work (multi-quarter roadmap alignment with partner teams) is no longer the highest-value activity
- **New core PM job**: How do we get something into users' hands this week? How do we shorten the path from idea to shipped?

Most PM candidates Cat Wu interviews haven't internalized this — they're optimizing for cross-team alignment rather than velocity. This is the number one mistake she sees.

### Three mechanisms for shipping at weekly velocity

**1. Set clear goals that rule things out.** LLMs are so general that without specific targeting, what you're building stays ambiguous forever. A strong goal names the exact user, exact problem, and exact use case — ruling out approaches immediately. Example: "Professional developers at enterprises should be able to safely reach zero permission prompts." Vague alternative ("reduce friction") invites endless scope expansion.

**2. Research Preview as a shipping mechanism.** Ship almost all features labeled as Research Preview. This signals to users that the feature is early, may change, and may not be permanent. It radically reduces the organizational commitment required to ship — you can get something in users' hands in a week or two without the full launch process.

**3. Create the cross-functional launch framework.** Engineers shouldn't have to negotiate with marketing and docs every time they want to ship. Anthropic's model: when an engineer feels a feature is dog-food ready, they post it in an "evergreen launch room." Marketing, docs, and DevRel are on-call for that channel and can turn around an announcement the next day. This is PM-built infrastructure; engineers use it without friction. PM's job is building this system, not doing the coordination manually each time.

### PRDs still exist — but only for the ambiguous and the long

For fast features: weekly metrics readouts + a shared team principles doc (key users, key use cases, key trade-offs) that everyone has internalized = no PRD needed. People make decisions on their own without asking PM. For genuinely ambiguous features: 1-pager covering goals, delightful use cases, and current failure modes. For infrastructure-heavy multi-month projects: full PRD. The middle category has shrunk dramatically.

### [Right Amount of AGI-Pilled](../concepts/right-amount-agi-pilled.md)

The hardest PM skill for AI-native products: calibrating how much to build for the model you have vs. the model you'll eventually have.

> "It is very hard to be the right amount of AGI-pilled. It's very easy to build the product for the super AGI strong model. The hard thing is figuring out for the current model, how do you elicit the maximum capability?"

- **Easy path**: Build for super-AGI. If the model is infinitely capable, you just need a text box — it adds its own tools, handles ambiguity, asks clarifying questions. No product complexity needed.
- **Hard path**: Build for the current model. Guide users to the golden path. Patch weaknesses in the product surface. Elicit maximum capability from what you actually have.

This is a rare skill. The best PMs see patterns in how users are hitting current model limits, set a near-term direction, and steadily execute — adjusting as model capabilities evolve faster or slower than expected.

### [Model Eats the Harness](../concepts/model-eats-the-harness.md)

As models improve, scaffolding added to compensate for prior model weaknesses becomes unnecessary — and should be actively removed.

Canonical example: the Claude Code to-do list.
- *Why it was added*: Early models would abandon multi-step tasks midway (fix 5 of 20 call sites, then stop). The to-do list forced state maintenance and task completion. Engineers had to prompt: "Did you finish everything on the list? You can't stop until you're done."
- *With Opus 4+*: The model naturally maintains and executes to-do lists without any prompting. The feature is now cosmetic (visible progress for users), not functional (required for model behavior).

Anthropic's practice: at each model launch, read the entire system prompt and ask "does the model still need this reminder?" Remove everything that's no longer compensating for a real weakness.

The more exciting direction: new models unlock features that couldn't ship before because accuracy wasn't high enough. Code review was tried multiple times with earlier models; with Opus 4.5/4.6 and Sonnet 4.6 it became reliable enough to run as a required gate before merging PRs. The product design was already built — the model just needed to catch up.

### Product taste is the scarce skill

> "As code becomes much cheaper to write, the thing that becomes more valuable is deciding what to write."

Tens of thousands of GitHub issues ask for every feature imaginable. The PM skill is knowing which ones are worth building and what the right UX is. This can come from any background — but it's rare. The reason engineering background is *currently* useful: better intuition for implementation cost, which feeds prioritization. But Cat Wu hedges with "for the next few months" — the valued skill set changes every few months as coding capability increases.

Most durable skill: first-principles thinking. Understand how the tech landscape is changing, identify what the team actually needs, jump in and fill the gap. Low ego about which hat you wear.

### Roles are merging — and that's the deliberate choice

Anthropic leans into engineers with product taste rather than a larger PM headcount:
- Many engineers go from seeing user feedback on Twitter → shipping a fix by end of week, with minimal PM involvement
- Nearly all PMs on the team have engineering backgrounds or actively ship code on Claude Code
- Designers are former front-end engineers

The trade-off Cat Wu names directly: **sacrificing product consistency**. Fast shipping produces overlapping features, unclear decision trees for new users, a sense of feature overload. Anthropic's answer: the `/powerup` command (opt-in onboarding that shows the 10 most important features out of 100). A divergence from their original "product should be intuitive enough to need no tutorial" principle — they bent the principle when evidence demanded it.

### Mission as decision tiebreaker — and how it differs from "focus"

Cat Wu distinguishes two things that get conflated:

- **Mission**: Teams willing to sacrifice their own OKRs in service of Anthropic's mission. Not just a mission statement — a genuine willingness to deprioritize your product's success for the company's. "If Claude Code failed but Anthropic succeeded, I would be extremely happy." This willingness enables fast cross-org decisions.
- **Focus**: Choosing what to build based on mission alignment. Prevents pursuing commercially interesting ideas that don't serve the mission.

The practical mechanism: when two priorities conflict, evaluate which better serves Anthropic's mission. Everyone accepts the decision. This is rare at company scale.

### What humans still uniquely provide

- **Common sense and EQ**: The thousand moving pieces of a product launch, stakeholder preferences, right communication venues, who needs to be on board and when. Models don't yet have this.
- **Product taste**: The judgment call on what's worth building.
- **Model calibration**: Knowing when the model is genuinely ready vs. when it needs more work.

### Automation philosophy: 95% is not an automation

If an automation doesn't work 100% of the time, you still need to supervise it — it's not real leverage. The last 5–10% takes real effort but is what makes the automation trustworthy. Push to 100% before treating it as leverage.

Counter-warning: there's a population of people spending more time customizing their AI workflow than shipping anything. Simple setups often work better than elaborate MCP/skill stacks. "The simple setups actually work better."

---

## Notable Quotes

> "It is very hard to be the right amount of AGI-pilled. It's very easy to build the product for the super AGI strong model. The hard thing is figuring out for the current model, how do you elicit the maximum capability?"

> "As code becomes much cheaper to write, the thing that becomes more valuable is deciding what to write."

> "The timelines for a lot of our product features have gone down from six months to one month and sometimes to even one day."

> "If Claude Code failed but Anthropic succeeded, I would be extremely happy."

> "Jobs are fake. If you understand the constraints, you can figure out what you can do and then just try to do it quickly, learn from the mistakes and apologize or fix them if you did something wrong."

> "If an automation doesn't work 100% of the time, it's not really an automation."

> "I think the simple setups actually work better."

> "The most important thing is to have this first principles thinking where you can figure out how the tech landscape is changing, what the team really needs from you, and just like jump in and fix that hole."

---

## Frameworks Introduced

- **[Right Amount of AGI-Pilled](../concepts/right-amount-agi-pilled.md)** — The calibration problem: build for current model capability, not superintelligence; eliciting maximum performance from what you have is the rare skill
- **[Model Eats the Harness](../concepts/model-eats-the-harness.md)** — Systematically remove scaffolding as models improve; each new model launch is an audit opportunity
- **Research Preview as shipping mechanism** — Label early features explicitly as Research Preview to dramatically lower the organizational commitment required to ship
- **Evergreen launch room** — A standing cross-functional channel where engineers post ship-ready features and marketing/docs/DevRel turn around announcements the next day; PM builds this, engineers use it frictionlessly
- **Mission as tiebreaker** — Use mission alignment (not just business metrics) to resolve competing priority decisions fast, with org-wide buy-in

---

## PM Relevance

1. **The weekly velocity doctrine is directly applicable to Copilot teams at Microsoft.** Most Microsoft PM teams operate on quarterly planning cycles with multi-team dependency maps. Cat Wu's three mechanisms (clear goals, Research Preview equivalent, evergreen launch process) are deployable at the team level without waiting for org-wide change. A "Research Preview" or "Copilot Preview" label for experimental features would reduce the political cost of shipping early — which is the real bottleneck in large organizations, not engineering capacity.

2. **"Right amount of AGI-pilled" is the defining calibration problem for Copilot product strategy.** Microsoft's Copilot teams face this exact tension: how much to build assuming current model capability vs. GPT-5/next generation? Cat Wu's insight is that building for super-AGI is the *lazy* option. The hard, valuable work is making current models perform at maximum capability for users today. This argues for investment in prompting architecture, user guidance, and golden-path design — not just waiting for the next model upgrade.

3. **Model Eats the Harness = audit Copilot scaffolding on every model upgrade.** Every time a new model ships in Azure OpenAI or GitHub Copilot, the right question is not just "what new capabilities does this unlock?" but "what existing scaffolding can we now remove?" Prompt engineering layers, orchestration rules, and compensatory UX elements designed for GPT-4-era weaknesses may now create friction by overriding behaviors the new model handles naturally. Removing them may actually improve performance.

4. **Product taste is what Microsoft should hire for, not just AI engineering chops.** The claim that taste > technical background (for product decisions) applies to Copilot PM hiring. The scarcest thing is judgment about what to build and how it should feel — not the ability to write prompts or orchestrate agents. As the technical barrier to prototyping drops to near-zero, taste becomes the differential.

5. **Mission-as-tiebreaker is a structure Microsoft product orgs mostly lack.** Microsoft has mission statements but they don't function as the decision tiebreaker Cat Wu describes. The Anthropic model — teams genuinely willing to deprioritize their own product's KRs in service of the broader mission — enables the cross-org fast decisions that produce this launch velocity. This is a cultural design question for Copilot leadership.

6. **Cowork's mental model** (code output → Claude Code; non-code output → Cowork) is useful competitive intelligence for Microsoft Copilot positioning. The split is clean and intuitive. Microsoft's equivalent question: when should users reach for Copilot in Word/Teams vs. GitHub Copilot vs. Azure AI? The lack of a clear answer creates confusion that slows activation at the same place Anthropic has clarified it.

7. **The Applied AI dossier workflow is a model for Microsoft CSM teams.** Anthropic's Applied AI team uses Cowork the night before customer meetings to pull all context (action items, open asks, latest ETAs from Slack) into a pre-meeting brief. Microsoft's Customer Success / FastTrack teams could replicate this exactly with Copilot for Sales. This is a concrete, deployable workflow — not just a concept.

8. **"Build products you actually use every day"** is the acid test for internal AI feature adoption at Microsoft. Cat Wu's framing is useful: there's a difference between AI that gets demoed and AI that delivers daily leverage. The question for any Copilot feature: is anyone on the product team using this every day for their actual job? If not, that's a signal.

---

## Entities Mentioned

- [Cat Wu](../entities/cat-wu.md) — Head of Product, Claude Code & Cowork, Anthropic
- [Anthropic](../entities/anthropic.md) — Developer of Claude, Claude Code, Cowork
- [Boris Cherny](../entities/boris-cherny.md) — Creator of Claude Code, tech lead (co-leads with Cat Wu)

## Concepts Touched

- [Right Amount of AGI-Pilled](../concepts/right-amount-agi-pilled.md) — Calibrating product vision to current vs. future model capability
- [Model Eats the Harness](../concepts/model-eats-the-harness.md) — Removing scaffolding as models improve
- [AI Evals](../concepts/ai-evals.md) — 10 great evals > 100 mediocre ones; PMs should build evals for ambiguous features; evals as product definition tool
- [Latent Demand](../concepts/latent-demand.md) — Cowork origin: non-technical users using a developer tool for non-coding tasks
