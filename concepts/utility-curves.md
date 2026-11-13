---
title: "Utility Curves"
type: concept
date_added: 2026-04-19
tags: [product-strategy, frameworks, design, microsoft-relevant]
sources: ["https://www.lennysnewsletter.com/p/slack-founder-stewart-butterfield"]
related: ["../podcasts/lenny-stewart-butterfield-slack.md", "../entities/stewart-butterfield.md"]
---

# Utility Curves

---

## Definition

A mental model from Stewart Butterfield for reasoning about feature investment and value delivery. Features don't exist as binary (have it / don't have it) — they exist on an **S-shaped curve** where the relationship between investment and value delivered is non-linear.

The curve:
- **Horizontal axis**: Investment — cost, effort, quality of implementation
- **Vertical axis**: Value delivered — utility, convenience, quality as experienced by the user
- **Shape**: Flat → steep → flat again (classic S-curve)

The three zones:
1. **Below threshold (first flat zone)**: Investment produces almost no value. The feature exists but isn't useful enough to matter. Users don't adopt it; they don't care it exists.
2. **The steep zone (inflection)**: A relatively small additional investment crosses the threshold and suddenly creates enormous value. This is where aha moments live.
3. **Past the cliff (second flat zone)**: Continued investment yields diminishing returns. You've extracted most of the value this feature can provide. Further improvement doesn't matter much.

---

## Why It Matters

**Features are almost always evaluated as binary**, but the decision of *how much* to invest in a feature is where most product mistakes happen:

- Teams add a feature that isn't good enough to cross the threshold → users don't adopt → team concludes "users don't want this" → they're wrong
- Teams keep investing in a feature past the cliff → diminishing returns → opportunity cost of not investing elsewhere
- Teams don't revisit shipped features → the quality bar moves (rising user expectations) → the feature slides back below threshold without anyone noticing

The second flat zone masquerades as success. A feature at the top of the curve can slide below the threshold over time as competitors improve or user expectations rise. **Most things get improved upon very infrequently. Some things get improved upon never.**

---

## Divine Discontent

Jeff Bezos' term: the quality bar moves continuously. Users who've seen a great checkout experience won't tolerate a mediocre one. Users who've seen a smart notification system won't tolerate a dumb one. The curve doesn't stay fixed — what was in the "good" zone two years ago may now be below the threshold of "acceptable."

The Google Calendar time zone picker: an app used by hundreds of millions of people, presents all time zones alphabetically by country. If you're in California and want to set a meeting in New York time, your first result for "East" is "Eastern Australia, New South Wales." This feature exists below the threshold of basic utility — it's harder to use than a mental model. Someone on the Google Calendar team likely thinks the feature is done (second flat zone). It's actually in the first flat zone because the implementation never cleared the threshold of usefulness.

Nobody switches from Google Calendar because of this. But the emotional tax accumulates. The negative emotional association ("I hate this thing that drives me bananas") reduces advocacy and increases susceptibility to switching when an alternative appears.

---

## The Key Questions

For any feature, ask:
1. **Where are we on the curve?** Have we cleared the threshold (do users actually get value from this)? Or have we only built the minimum scaffold?
2. **Has the curve moved?** Was this feature adequate when built but now sub-threshold because expectations have risen?
3. **Are we in diminishing returns?** Is further investment going to meaningfully move the curve, or are we polishing something that's already past its plateau?
4. **What's the threshold?** What's the minimum investment required to get into the steep zone — and are we committed to reaching it, or are we going to stop short and wonder why nobody uses it?

The hardest insight: if you're going to build a feature, commit enough to clear the threshold. A feature that almost works is often worse than not having the feature at all — it adds complexity, creates confusion, and poisons users against trying again.

---

## Examples

**Hammer quality** (Butterfield's example): If the handle breaks on impact, the hammer is useless. A slightly stronger handle: still useless. Junk, junk, junk — then suddenly, good, great, excellent. Then it doesn't matter if you make it stronger; you're past the cliff.

**Database tables**: Building the users table in a database generates zero user value. It's all necessary below-threshold work to eventually get to the steep zone.

**Slack notifications for new accounts**: First instinct was "notify only for DMs and @mentions." But new users need to understand the product works at all. The "correct" default was too far up the curve — users hadn't yet understood the product. They set an intermediate default (all notifications) to get people through onboarding, then prompted them to switch once they'd received enough messages to understand context.

**Account creation flows, checkout flows, forgot password**: These are features that "ship once and are considered done" in most organizations, while the quality bar in the broader ecosystem keeps rising. Every major product has these features quietly sliding back below the threshold.

---

## PM Application

For a Senior Director of PM at Microsoft:

1. **Copilot feature investment threshold**: For any Copilot feature under development, ask explicitly: are we committing enough investment to clear the threshold? Half-built AI features that don't quite work are worse than no feature — users try them, fail, and conclude AI doesn't work. This is the most dangerous failure mode for Copilot adoption. Either go far enough to clear the threshold or don't launch.

2. **Roadmap reviews**: Reframe feature discussions from "do we have this?" to "where on the curve are we, and is it worth getting to the threshold?" This changes the conversation from binary (yes/no) to investment sizing (how much to actually make this good).

3. **Feature maintenance as a strategy**: Create a regular audit of features that "shipped and are done." Identify which ones are sliding back below threshold due to rising user expectations. Some of these will be worth re-investing in; others should be cut. Most orgs have no process for this.

4. **User research as threshold detection**: Watch users attempt a feature. If they attempt it, don't get value, and give up — you're below threshold. If they attempt it, get value, and come back — you're in the steep zone. The behavior tells you more than a survey.

5. **Divine discontent as team culture**: Butterfield's quote: "I feel like what we have right now is just a giant piece of shit... if you can't see almost limitless opportunities to improve, you shouldn't be designing the product." This orientation — perpetual dissatisfaction as a design culture — is what prevents features from sliding back below the threshold unnoticed.

---

## Sources

- [Slack Founder: Mental Models for Building Products People Love](../podcasts/lenny-stewart-butterfield-slack.md) (Stewart Butterfield, 2025-11-20)
