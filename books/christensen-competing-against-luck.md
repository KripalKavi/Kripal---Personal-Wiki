---
title: "Competing Against Luck: The Story of Innovation and Customer Choice"
type: book
date_added: 2026-04-19
tags: [product-strategy, frameworks, design, innovation, microsoft-relevant]
sources: ["Clayton M. Christensen et al., Competing Against Luck: The Story of Innovation and Customer Choice (2016)"]
related: ["../podcasts/lenny-google-ai-mode-robby-stein.md", "../entities/robby-stein.md", "../concepts/we-dont-sell-saddles-here.md", "../concepts/latent-demand.md"]
---

# Competing Against Luck

**Author**: Clayton M. Christensen, Taddy Hall, Karen Dillon, David S. Duncan
**Year**: 2016
**Recommended by**: Robby Stein (Lenny's Podcast, 2025-10-10) — cited as the framework behind Google's AI Mode product philosophy

---

## Summary

Christensen's definitive articulation of the Jobs to Be Done (JTBD) theory: customers don't buy products — they "hire" them to do a job in their lives. Product innovation fails at staggering rates not because of poor execution, but because teams build solutions around the wrong understanding of why customers buy. The book reframes the entire product development task: before asking "what should we build?", ask "what job is the customer trying to get done?"

---

## Key Ideas

### The Milkshake Story
The canonical JTBD story: a fast-food chain wanted to increase milkshake sales. Standard approaches (surveys, demographics, focus groups) gave conflicting, unhelpful answers. Researchers discovered the real job: morning commuters hired milkshakes to keep them occupied, stave off hunger until lunch, and provide something interesting to do with one hand while driving. The competitors weren't other milkshakes — they were bananas (too quick), donuts (too messy), and bagels (too dry). Understanding the job revealed the right product improvements (thicker, more viscous, takes longer to consume) that demographics and features never would have.

### Jobs Are Functional, Emotional, and Social
Every job has three dimensions:
- **Functional**: the practical task to be accomplished
- **Emotional**: how the customer wants to feel while doing it
- **Social**: how the customer wants to be perceived by others while doing it

Most product teams only solve for the functional dimension. But emotional and social jobs are often the decisive differentiators — and the least understood. Uber didn't win on the functional job (getting a ride) — it solved the emotional job (the anxiety and awkwardness of hailing a cab) and the social job (not looking cheap or clueless in front of colleagues).

### "Hire" and "Fire" Language
Customers aren't loyal to products — they hire products when the job arises and fire them when something else does the job better. This reframe changes what you monitor: instead of tracking customer satisfaction with your product, track whether customers are experiencing the job and choosing your product to do it. The insight gap: most products get "fired" for reasons unrelated to their core functionality (the experience of hiring them is too complex, the social context is wrong, etc.).

### The Progress-Making Force Model
Why do customers switch to a new product? Four forces are always at work:
1. **Pushing** from the old solution (frustration, limitation)
2. **Pulling** toward the new solution (the appeal of the new way)
3. **Anxieties** about switching (learning cost, uncertainty)
4. **Habit** / attachment to the old way

All four must be understood to design a successful switch. Advertising typically addresses forces 1 and 2 and ignores 3 and 4 — which is why customers who are frustrated with the old solution and excited about the new one still don't switch.

### Big Hire vs. Little Hire
Customers make two hires: the *big hire* (buying the product) and the *little hire* (actually using it in the moment). Many products succeed at the big hire and fail repeatedly at the little hire — the customer has it but doesn't reach for it. Activation and habit formation are "little hire" problems. In AI products, this maps to the difference between signing up for Copilot and actually using Copilot in your workflow.

### Non-Consumption Is the Biggest Competitor
For most products, the primary competitor is not a rival product — it is *doing nothing*. Most new products expand the market by addressing non-consumption, not by stealing share from competitors. The question "who is your competition?" usually has a wrong answer when the real answer is "the status quo."

---

## Quotable Lines

> "Customers don't buy products. They hire them to do a job."

> "The milkshake's competition was not other milkshakes. Its competition was boredom and hunger."

> "Innovation fails most often not because it isn't good, but because it was built for the wrong job."

> "If you don't understand the job your product was hired to do, you're competing against luck."

---

## PM Application

For a Senior Director of PM at Microsoft:

1. **Robby Stein's direct application to Search**: Stein cited Christensen explicitly — the job of search is not "find a link." It's "answer my question and help me accomplish my goal." AI Mode doesn't change the job; it expands what Search can do *for* that job. This is the correct lens for evaluating AI integration in any existing Microsoft product: does this help users accomplish the job better, or does it change the job?

2. **The Copilot "big hire vs. little hire" gap**: Copilot has strong acquisition (big hire) but known activation challenges (little hire). JTBD frames this precisely: users hired Copilot for a job (reduce information overload, draft faster, summarize meetings), but when the little hire moment comes ("I should use Copilot for this"), they don't. The fix isn't more features — it's designing for the little hire moment: what is the trigger that makes someone reach for Copilot?

3. **Non-consumption as Copilot's real competitor**: For most Copilot use cases, the primary competitor is not ChatGPT or Google Gemini — it's doing the task manually. Understanding non-consumption means understanding why the job gets done without AI: habit, trust, time to learn the tool, unpredictability of output. Each of these is an anxiety in the progress-making force model.

4. **Functional/Emotional/Social for M365 Copilot**: The functional job of Copilot in email is "summarize and draft faster." The emotional job is "feel in control, not overwhelmed." The social job is "appear competent and responsive to colleagues." Microsoft's marketing and product design mostly addresses the functional layer. The emotional and social layers are under-invested.

5. **JTBD for the Copilot+ PC product category**: What job does a Copilot+ PC do that a regular PC doesn't? If the answer is a list of features (NPU, Recall, real-time translation), those are product descriptions, not jobs. The JTBD framing forces the harder question: what does a customer hire a Copilot+ PC to do that they currently can't do well, or that they're currently hiring something else (or nobody) to do?

---

## Related Concepts

- [Latent Demand](../concepts/latent-demand.md) — JTBD and latent demand are complementary: JTBD asks what job customers are hiring for; latent demand asks what jobs they're already doing outside your product
- [We Don't Sell Saddles Here](../concepts/we-dont-sell-saddles-here.md) — Both frameworks say: describe the transformation (the job), not the product
