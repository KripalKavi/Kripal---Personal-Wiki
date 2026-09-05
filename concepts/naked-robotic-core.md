---
title: "Naked Robotic Core"
type: concept
date_added: 2026-05-15
tags: [product-strategy, design, frameworks, microsoft-relevant]
sources: ["https://www.lennysnewsletter.com/p/why-cultivating-agency-matters-more"]
related: ["../podcasts/lenny-max-schoening-agency-over-skills.md", "../entities/max-schoening.md", "../concepts/tiny-core.md", "../concepts/obviously-good.md", "../concepts/first-ten-percent-free.md"]
---

# Naked Robotic Core

## Definition

After a period of exploration in which multiple competing primitives are allowed to grow, **the hard work of consolidation** — pruning the evolutionary branches back to the single, simple idea that should outlive them. The "naked robotic core" is the irreducible, generic version of the idea that the surface variants were all approximating.

[Max Schoening](../entities/max-schoening.md):

> "We let a bunch of different ideas grow. We look at how they work. But then you do have to do the hard work at consolidating it back into the naked robotic core of that idea. And that's hard, because you have to be okay with perhaps then shipping the next thing slightly delayed as you reconcile."

---

## Why It Matters

Increased shipping velocity + parallel experimentation (enabled by [First 10% Is Free](../concepts/first-ten-percent-free.md)) generates **primitive sprawl**: many features that do conceptually similar things in surface-different ways. Without consolidation, the product accumulates UX debt that compounds:

- Users can't predict which primitive does what
- Each primitive has incomplete coverage of the underlying idea
- Engineering complexity multiplies
- The team is forced to maintain six versions of one thing

Schoening's examples:
- **Notion**: six automation primitives (counting agents). Schoening admits: *"We let a bunch of different ideas grow."*
- **Claude desktop**: three tabs (co-work, code, chat). *"Why do we have six automation primitives? Well, because someone has to sit down and reconcile them and figure out what's actually the core simple thing that should outlive the other evolutionary branches of that same idea."*

This is the *consolidation discipline* paired with the *exploration discipline*. Without it, you ship demos forever and never get to obviously good.

---

## The Painful Cost

The reason consolidation gets deferred:

> "You have to be okay with perhaps then shipping the next thing slightly delayed as you reconcile."

Consolidation produces **no new feature**. The next launch slips while the team reconciles. Stakeholders see a quiet quarter. The reward for consolidation is invisible from the outside — until later, when the surviving primitive enables a year of compounding work that the sprawl version couldn't have supported.

This is the unsexy product-leader work that distinguishes great organizations from prolific ones.

---

## The Relationship to Tiny Core

[Tiny Core](../concepts/tiny-core.md) is the **principle**: every great product has one exceptional primitive. **Naked Robotic Core is the operational discipline that produces the tiny core** when divergent exploration has obscured it.

You almost never find the tiny core on the first try. You explore multiple candidates, ship them, see what users do, then consolidate back. The consolidation *is* the moment the tiny core becomes legible to the organization.

Without naked-robotic-core consolidation, you accumulate primitives forever and never converge on the tiny core. The product feels chaotic because *it is.*

---

## What "Naked Robotic" Means

The metaphor is specific. **Naked** = stripped of skinning, branding, surface differentiation. **Robotic** = mechanical, simple, predictable. The naked robotic core is the lowest-level mechanic that does the actual work — without the surface ornamentation each evolutionary branch added.

Example for Notion's automation: each primitive (database automations, button automations, formula automations, AI automations, agent automations, etc.) is a *surface skin* on the underlying mechanic of "trigger → condition → action." The naked robotic core is "trigger → condition → action," presented as one primitive that subsumes the others.

---

## Related to Adjacent Concepts

- **[Tiny Core](../concepts/tiny-core.md)** — the principle; Naked Robotic Core is the discipline that produces it after exploration.
- **[Obviously Good](../concepts/obviously-good.md)** — products feel obviously good when they have a single primitive; they feel chaotic when they have six versions of one primitive.
- **[First 10% Is Free](../concepts/first-ten-percent-free.md)** — cheap exploration makes sprawl inevitable; consolidation discipline becomes more important, not less.
- **Shots on goal** — pair: more shots produce more divergence; more divergence requires more consolidation.

---

## PM Application

For a Senior Director of PM at Microsoft:

1. **Audit Copilot for primitive sprawl.** Microsoft has many entry points to "AI assistant": chat panel, side panel, in-line completions, agent builder, autonomous agents, Copilot Studio, Copilot Pages, etc. Some of these are different products; some are evolutionary branches of one product without a naked robotic core. Identify which is which. The branches need consolidation; the products need to coexist.

2. **Plan an "ugly quarter."** Schedule a deliberate consolidation period where no new features ship and a sprawled surface gets reconciled to its naked robotic core. The cost is visible (slow launches). The benefit is hidden but compounding (a year of accelerated work on the surviving primitive).

3. **The 6-primitive smell test.** If your team has more than three ways to do the same conceptual thing, the consolidation question is overdue. Schoening's Notion has six; he calls this consolidation debt. M365 has multiple ways to "summarize a document with AI." If users can't predict which one to use, consolidation is overdue.

4. **Consolidation requires *killing your darlings*.** Each evolutionary branch had a reason it existed; an internal champion. Naked robotic core means most of those champions don't get to keep their version. This is org-political work, not just product work. The senior PM's job is making that decision and absorbing the cost.

5. **Beware "we'll consolidate later."** Consolidation that doesn't have a forcing function never happens. Either schedule it explicitly, or it becomes permanent debt. The forcing function can be: a major release, a redesign, a strategy pivot, or a senior leader's mandate. Pick one.

6. **Apply to the launch-readiness review.** A reasonable obviously-good check: *"Does this feature duplicate a primitive we already have? If yes, does it justify being a parallel primitive, or should it consolidate into the existing one?"* Default to consolidation.

---

## Sources

- [Lenny's Podcast — Max Schoening](../podcasts/lenny-max-schoening-agency-over-skills.md) — primary articulation, 2026-05-03

## Related

- [Tiny Core](../concepts/tiny-core.md)
- [Obviously Good](../concepts/obviously-good.md)
- [First 10% Is Free](../concepts/first-ten-percent-free.md)
