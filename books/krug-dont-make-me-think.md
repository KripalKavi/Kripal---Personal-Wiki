---
title: "Don't Make Me Think"
type: book
date_added: 2026-04-19
tags: [product-strategy, design, frameworks, ux, microsoft-relevant]
sources: ["Steve Krug, Don't Make Me Think (2000; 3rd ed. 2014)"]
related: ["../podcasts/lenny-stewart-butterfield-slack.md", "../entities/stewart-butterfield.md"]
---

# Don't Make Me Think

**Author**: Steve Krug
**Year**: 2000 (3rd ed. 2014)
**Recommended by**: Stewart Butterfield (Lenny's Podcast, 2025-11-20)

---

## Summary

The definitive usability guide for digital products. Krug's central argument: the most important principle of web/product design is that users should never have to stop and think about what they're doing. Every moment of uncertainty or confusion is a cognitive cost — and those costs accumulate until users give up. Most product design problems are comprehension problems, not feature gaps.

---

## Key Ideas

### The Core Principle
"Don't make me think" — literally. Every element of a design should be obvious without explanation. If a user has to stop and ask "what does this do?" or "what should I do next?", the design has failed at that point. Users should be able to navigate by intuition, not by reading.

### Cognitive Load as the Real Friction
Most product teams talk about "reducing friction" and count clicks. Wrong metric. Clicks are fine; confusion is not. A 10-click flow where every click is obvious is better than a 3-click flow where one step requires thought. The cost is metabolic — literally glucose expenditure — but more importantly, it's emotional. Confusion makes users feel stupid. That feeling attaches to the product.

### Satisficing, Not Optimizing
Users don't read pages — they scan them. They don't make optimal choices — they pick the first option that seems reasonable ("good enough"). They don't figure things out — they muddle through with the minimum understanding needed to proceed. Design for how people actually use products, not how we'd like them to.

### The Trunk Test
Drop a user on any page in your product with no context. Can they answer: What site/product is this? What page am I on? What are the major sections? What can I do here? What's important? Where am I relative to where I started? If not, the page fails basic wayfinding. Most products fail for non-authenticated users who arrive from search or sharing.

### Happy Path vs. All Paths
Most designers obsess over the happy path. Krug's emphasis: design for confused users, not confident ones. The error states, the empty states, the unexpected paths — these are where users abandon. The happy path takes care of itself; the confused path requires explicit design work.

### Testing: One User Per Week Beats Perfect Research
Krug's practical recommendation: usability testing doesn't need to be rigorous or large. Watching one real user use your product for one hour every week tells you more than quarterly research sprints. The goal isn't statistical significance — it's catching the obvious embarrassments before they ship.

---

## Quotable Lines

> "Don't make me think."

> "Get rid of half the words on each page, then get rid of half of what's left."

> "Your worst enemy is the word 'obvious'... what's obvious to you may not be obvious to everyone."

> "If something is hard to use, I just don't use it as much." — *how users actually respond to confusing design*

---

## PM Application

For a Senior Director of PM at Microsoft:

1. **The Butterfield validation**: Butterfield cited this as *the* correct design mantra, explicitly over "reduce friction." His argument: 70-80% of product design work lives in the comprehension problem. Copilot's activation challenge is entirely a comprehension problem — users don't use it more because they don't know what to ask, not because sign-up is slow.

2. **The Trunk Test for Copilot surfaces**: Apply this to every Copilot entry point in M365. Drop a user on the Copilot pane in Word, Teams, or Outlook. Without any prior knowledge, can they answer "What can I do here?" and "What should I do first?" Most current implementations fail this test.

3. **Error states and empty states are where Copilot loses users**: When Copilot fails (wrong answer, empty response, not enough context), what happens next? These moments likely drive most abandonment. The happy path (Copilot answers correctly the first time) already works. The confused path needs explicit design investment.

4. **"Get rid of half the words"**: Applied to Copilot prompts, onboarding copy, and feature description text. Every word in a UI is a word a user might have to read. The less there is, the less they can misunderstand.

5. **Testing frequency**: Krug's "one user per week" principle argues against large quarterly research efforts and for lightweight, continuous observation. For Copilot feature teams, this means someone watches a real user use the product every week — not waiting for quarterly research cycles.

---

## Related Concepts

- [We Don't Sell Saddles Here](../concepts/we-dont-sell-saddles-here.md) — Comprehension is the saddle problem; users can't understand the transformation if the product makes them think
- [Latent Demand](../concepts/latent-demand.md) — What users don't do because of comprehension failures is latent demand
