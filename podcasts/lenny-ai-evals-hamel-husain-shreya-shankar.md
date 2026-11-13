---
title: "Why AI Evals Are the Hottest New Skill"
type: podcast
date_added: 2026-04-19
tags: [ai, evals, product-quality, ai-development, frameworks, microsoft-relevant]
sources: ["https://www.lennysnewsletter.com/p/why-ai-evals-are-the-hottest-new-skill"]
related: ["../entities/hamel-husain.md", "../entities/shreya-shankar.md", "../concepts/ai-evals.md"]
---

# Why AI Evals Are the Hottest New Skill

**Show**: Lenny's Podcast
**Guests**: [Hamel Husain](../entities/hamel-husain.md) and [Shreya Shankar](../entities/shreya-shankar.md), AI eval researchers and educators
**Host**: Lenny Rachitsky
**Published**: 2025-09-25
**Source**: https://www.lennysnewsletter.com/p/why-ai-evals-are-the-hottest-new-skill

---

## Summary

Hamel Husain and Shreya Shankar argue that systematic evaluation frameworks have become the foundational skill for building reliable AI products — replacing gut-feel and "vibes" testing with a rigorous methodology borrowed from qualitative research. The episode walks through a full eval development process, from initial error analysis to ongoing maintenance, and reframes evals as a PM deliverable rather than a purely engineering concern.

---

## Key Takeaways

### Start with error analysis — always
- Before writing a single eval, manually review real user traces (actual inputs and outputs from your system)
- This upstream investigation reveals what is *actually* breaking vs. what you *assume* is breaking
- Skipping this step leads to evals that test the wrong things — a common and costly mistake
- The traces are the ground truth; your intuitions about failure modes are usually wrong or incomplete

### The qualitative coding methodology: open coding → axial coding
- **Open coding**: Go through traces and tag raw failure modes as you see them — no categories yet, just labels (e.g., "missed user intent," "wrong tone," "hallucinated fact," "incomplete response")
- **Axial coding**: Group the raw tags into 5–6 higher-level failure categories that represent the core dimensions of how your system fails
- **Theoretical saturation**: Keep analyzing traces until new traces stop producing new failure types — this is your signal that you've captured the space
- This methodology comes from social science qualitative research — it's designed to surface patterns from messy real-world data without imposing pre-existing structure

### The Benevolent Dictator principle
- One person should own and lead eval development for a given product or feature
- This ensures consistency in judgment calls when coding failure modes and calibrating LLM-as-judge prompts
- Without a single accountable owner, different people's interpretations of "good" vs. "bad" contaminate the data and make evals unreliable

### Two types of evals — and when to use each
- **Code-based evals**: Deterministic rules checking specific outputs (e.g., "does the response contain a citation?", "is the JSON valid?"). Fast, cheap, fully reliable — but limited in scope
- **LLM-as-judge**: Uses another LLM to evaluate output quality against a rubric. Flexible and scalable, but requires calibration: the judge's ratings must be validated against human judgments before you trust it
- Most robust systems use both: code-based for hard constraints, LLM-as-judge for quality dimensions

### Evals as the new PRDs
- Coined by Brendan Foody: well-crafted eval prompts are living product requirements documents
- If you can write a precise eval for a behavior, you've actually specified what you want — which is harder than it sounds
- Implication: the act of writing evals forces clarity of requirements in a way that traditional prose specs don't
- Evals continue validating those requirements automatically as the model or system changes over time

### Low ongoing overhead once established
- After initial setup, ongoing eval maintenance requires ~30 minutes per week
- This makes systematic evals achievable for PM-led teams, not just ML engineering teams
- The upfront investment (building the error taxonomy and initial eval suite) is the hard part

### Statsig acquisition as an industry signal
- OpenAI's acquisition of Statsig signals that evaluation and testing infrastructure is now considered foundational, not auxiliary
- Companies that don't build eval infrastructure are accumulating technical and product debt they'll pay later

---

## Notable Quotes

> "Evals are the new PRDs." — Brendan Foody (cited by guests)

> Start with error analysis — "not what you assume is broken, but what's actually breaking in production."

---

## Frameworks Introduced

- **Open coding / Axial coding**: Qualitative research methodology applied to AI failure analysis. See [AI Evals](../concepts/ai-evals.md).
- **Theoretical saturation**: The point at which new data stops producing new patterns — signals sufficient coverage for eval writing.
- **LLM-as-judge**: Using a second LLM to evaluate the outputs of the primary LLM, calibrated against human judgment.
- **Benevolent Dictator**: Single eval owner who ensures consistent interpretation and judgment across an eval suite.

---

## PM Relevance

1. **Evals as a PM artifact**: "Evals as PRDs" is a direct call to action. Writing eval criteria before writing feature specs forces you to articulate exactly what "good" looks like — something prose requirements rarely achieve. For Copilot features, this means defining success in terms of evaluable output quality, not just feature existence.

2. **Error analysis is product research**: The open/axial coding methodology doesn't require ML expertise — it requires the same skill PMs already use to synthesize user feedback. Reviewing AI output traces and categorizing failures is a PM-ownable activity, not just an engineering one.

3. **Microsoft eval infrastructure gap**: OpenAI acquiring Statsig is a direct signal. Microsoft should be asking: do Copilot products (M365 Copilot, GitHub Copilot, Azure AI) have robust eval infrastructure? Is quality measured systematically before every release, or are teams relying on internal dogfooding and user complaints?

4. **Evals gate quality in fast-moving AI products**: In traditional software, tests catch regressions. In AI products, evals catch model behavior drift — when a new model version, new prompt, or new grounding data changes outputs in unintended ways. Every Copilot release without evals is a ship-and-hope deployment.

5. **PM as eval author on the team**: The ~30 min/week maintenance claim means PMs can credibly own eval suites for their product areas. This is a new PM skill worth developing — teams that have PMs who can write and interpret evals will move faster and ship higher-quality AI features.

---

## Entities Mentioned

- [Hamel Husain](../entities/hamel-husain.md) — AI researcher, eval educator
- [Shreya Shankar](../entities/shreya-shankar.md) — AI researcher, eval educator

## Concepts Introduced

- [AI Evals](../concepts/ai-evals.md) — Systematic evaluation framework for AI products
