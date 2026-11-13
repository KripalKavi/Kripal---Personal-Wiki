---
title: "Latent Demand"
type: concept
date_added: 2026-04-19
tags: [product-strategy, frameworks, ai, product-discovery, microsoft-relevant]
sources: ["https://www.lennysnewsletter.com/p/head-of-claude-code-what-happens"]
related: ["../podcasts/lenny-claude-code-boris-cherny.md", "../entities/boris-cherny.md"]
---

# Latent Demand

---

## Definition

**Latent demand** is the signal that users give you by using your product in ways you never designed for — hacking around its edges to accomplish something the product wasn't built to do. That unsupported behavior reveals real unmet need. Build a product that serves it directly, and adoption will be fast because the demand is already proven.

Boris Cherny calls this "the single most important principle in product."

---

## Why It Matters

The hard part of product development isn't building — it's knowing what to build. Most product decisions are made by extrapolating from vision, competitor analysis, or customer interviews, all of which are noisy. Latent demand is a cleaner signal: users are already paying the cost of a workaround. That's revealed preference, not stated preference. The gap between what the product was built for and what users are actually doing with it is your product roadmap.

---

## Two Dimensions

### 1. Traditional Latent Demand — What Users Are Doing
Find the workaround. Where are users hacking your product to accomplish something it wasn't designed for?

**Examples:**
- **Facebook Marketplace**: 40% of Facebook Group posts were people buying and selling. Groups weren't designed for commerce — but people were using them for it anyway. Marketplace was obvious from this signal.
- **Facebook Dating**: 60% of profile views were between opposite-gender non-friends. The product wasn't designed for dating, but users were using it to scope each other out. Dating feature followed.
- **Anthropic Cowork**: Non-technical users were running Claude Code (a developer terminal tool) to analyze their genome, recover corrupted wedding photos, grow tomato plants, analyze MRIs. The demand for an agentic tool for non-developers was already there — Cowork was built to serve it. Built in 10 days.

**How to find it**: Track what users do *after* your product fails to do what they wanted. Look for unexpected use patterns in analytics. Watch support tickets for requests the product can't fulfill. Look for hacks, workarounds, and creative misuse.

### 2. Modern Latent Demand — What the Model Is Trying to Do
A newer dimension specific to AI products. Not just what users are doing, but what the model *itself* is trying to do when given latitude.

Traditional AI product design: put the model in a box. Define the workflow. Constrain the model to a specific function in a larger system.

Claude Code's inversion: the product IS the model. Minimal scaffolding. Give it tools. Let it decide how to use them. This design was grounded in observing what the model naturally did when given latitude — and building the product around that behavior rather than against it.

In research terms, this is called "being on distribution" — not fighting what the model naturally wants to do, but finding that natural behavior and building around it.

**Practical implication**: If your AI feature forces users through a rigid flow, you're probably fighting the model's natural behavior. Watch what the model does when given more freedom than your product currently allows. That behavior is a product signal.

---

## The Discovery Process

1. **Instrument the workarounds**: Build analytics that can detect when users are using the product in unanticipated ways — unusual query patterns, feature combinations, usage outside intended flows
2. **Watch the hacks**: Pay attention to power users doing creative things; they're early signals of demand
3. **Respond fast**: Boris's practice — when someone reported a workaround use case, he'd fix/build for it within minutes. Fast response encourages more signal.
4. **For AI products, give the model latitude in internal testing**: Watch what it tries to do when you give it tools and a goal without a rigid workflow. The emergent behaviors are product directions.

---

## PM Application

For a Senior Director of PM at Microsoft:

1. **Copilot latent demand audit**: What are users doing with Copilot that you didn't design for? What are they asking that it can't do but they keep trying? Each of those failures is a product brief. This is more valuable than most user research.

2. **Cowork-style discovery for Microsoft AI**: Before building the next Copilot feature, spend a week reading actual user sessions. What are users attempting that the product refuses or fails at? That's your backlog.

3. **The model's latent demand for Azure AI**: When customers use Azure OpenAI without rigid guardrails in early prototypes, what do they build? What does the model try to do that your current product architecture prevents? Those observations should feed the Azure AI platform roadmap.

4. **Fast-response feedback loop as a signal amplifier**: Boris's practice of responding to user feedback within minutes increased the volume of feedback dramatically. The speed of response signals that feedback matters — and users give more of it. Consider how this applies to Copilot feedback channels.

---

## Sources

- [Head of Claude Code: What Happens After Coding Is Solved](../podcasts/lenny-claude-code-boris-cherny.md) (Boris Cherny, 2026-02-19)
