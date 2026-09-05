---
title: "Reach Test"
type: concept
date_added: 2026-05-27
tags:
  - ai
  - product-strategy
  - activation
  - frameworks
  - microsoft-relevant
sources:
  - https://www.lennysnewsletter.com/p/the-ai-paradox-dan-shipper
related:
  - ../podcasts/lenny-dan-shipper-ai-paradox.md
  - ../entities/dan-shipper.md
  - ../concepts/ride-the-model.md
  - ../concepts/ai-product-activation.md
  - ../concepts/utility-curves.md
---

# Reach Test

## Definition

The **reach test** is Dan Shipper's adoption diagnostic for AI products, used internally at Every:

> "One of the things that we talk about internally is what I call the reach test, which is like, when you wake up in the morning, do you reach for it organically?"

The test is binary: when the user begins their day, do they spontaneously go to the product, or do they have to be reminded? If it's the former, the product has crossed into habit. If it's the latter — even if the user *likes* the product, even if they say they will use it more, even if the usage metrics look promising — it has not crossed.

## Why It Matters

Most AI-product engagement metrics are vanity-prone. Daily Active Users captures coerced opens. Asked-a-prompt captures one-shot curiosity. Time-in-product captures hesitation as much as engagement. The reach test is harder to game because it captures a *behavior the user initiates*, in the absence of any prompt or reminder.

For an AI product that intends to become part of how someone works, the reach test is the only metric that matters. Pre-reach: the product is a periodic novelty. Post-reach: the product is a workflow component. The gap between those two states is the activation gap, and most AI products live in the pre-reach state without realizing it because their dashboards show "engagement."

The test also distinguishes between *"the user said they liked it"* (qualitative noise that doesn't predict retention) and *"the user reaches for it"* (behavior that does). It's the AI-era analog to Stewart Butterfield's [Utility Curves](utility-curves.md) test — if a feature is below the value threshold, it produces zero outcome no matter what; the reach test detects when a product crosses the threshold for a specific user.

## How To Apply

1. **Don't ask users if they reach for it.** Observe whether they do. Stated preferences and revealed preferences diverge on this.
2. **Track first-action-after-laptop-open.** Per user, per day. What is the first product they open without being prompted by a calendar event, a notification, or a habit external to your app?
3. **Distinguish ride-the-model reach from product-loyalty reach.** Shipper himself currently *reaches* for Codex; he previously reached for Claude Code. The reach is real but the loyalty is to the frontier, not to the brand. See [Ride the Model](ride-the-model.md).
4. **Don't conflate reach with retention.** A user can reach for a product daily for three weeks and then stop. Reach is a strong leading indicator but not a guarantee. Pair it with cohort retention.
5. **Watch the *anti-reach* signal.** If users were reaching and stop, that's a much stronger negative signal than non-adoption. Something specific changed — a new release degraded a capability, a competitor crossed their threshold, the use case completed.

## Examples

- **Codex for Shipper** — Codex passes his reach test now; Claude Code passed it a year ago. *"I think Codex right now, it's my daily driver. I spend all my time in it, basically. I flip to Claude every once in a while."* The reach moved with the frontier capability.
- **The senior engineer benchmark** — every new model gets the same prompt the moment it ships. The benchmark passes the reach test for Shipper (he reaches for the new model on day one).
- **Email-in-Codex** — *"I've been at inbox zero for 10 days straight now, which if you know me, is crazy. I'm never like this, and that's because I literally just have Codex gather all my emails."* The Codex email workflow passed his reach test and changed a behavioral pattern that had previously been resistant to change.

## PM Application

For a Senior Director of PM at Microsoft:

1. **Make "reach" the Copilot North Star metric — not asked-a-prompt, not DAU, not seat utilization.** Per-user, per-day: when the user opens M365 in the morning, is Copilot the first surface they engage? If not, the seat license is at risk regardless of what other dashboards show. Instrument it. The dashboard becomes uncomfortable; that's the point.

2. **Audit existing engagement metrics against the reach test.** Many Copilot product reviews show strong engagement on metrics that are downstream of forced exposure (banners, recommendations, in-product nudges). The reach test strips this away. If a feature only sees engagement when promoted, it isn't part of the workflow.

3. **Use anti-reach as the canary.** When a Copilot release ships, monitor for drops in reach in the cohort of users who *had* been reaching. A drop after a release is the strongest signal that the release degraded something they were depending on. Faster diagnosis than waiting for churn or NPS.

4. **For GitHub Copilot and Codex-equivalent products, the reach test is the only fair comparison.** Don't compare *"users who tried Copilot"* to *"users who tried Codex."* Compare *"users who reach for Copilot when they sit down"* to *"users who reach for Codex when they sit down."* That is the workspace question. Shipper himself is currently in the Codex column. That should be uncomfortable.

5. **Be willing to lose reach battles to win the next one.** The reach moves with the frontier. If a Microsoft release temporarily loses reach to a competitor's better release, [Ride the Model](ride-the-model.md) and try to win it back on the *next* release rather than redesigning everything to prop up the losing one.

## Connection to Other Concepts

- **[Ride the Model](ride-the-model.md)** — the reach test detects whether your riding is sticking. If you ride the model and it doesn't pass the reach test, the application case isn't there yet.
- **[AI Product Activation](ai-product-activation.md)** — the reach test is the activation-completion signal for AI products. Pre-reach = pre-activation.
- **[Utility Curves](utility-curves.md)** — Butterfield's "if it's below the value threshold, you get zero output" framing. Reach is the binary value-threshold detector at the user level.
- **[Automation Is a Lie](automation-is-a-lie.md)** — the reach test sorts agent features that the user *chooses* from agent features that the user *tolerates*. The lie-zone is dominated by the tolerated category.

## Sources

- [The AI Paradox — Dan Shipper on Lenny's Podcast](../podcasts/lenny-dan-shipper-ai-paradox.md) — 2026-05-24, primary articulation

## Related

- [Ride the Model](ride-the-model.md)
- [AI Product Activation](ai-product-activation.md)
- [Utility Curves](utility-curves.md)
