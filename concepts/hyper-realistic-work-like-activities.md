---
title: "Hyper-Realistic Work-Like Activities"
type: concept
date_added: 2026-04-19
tags: [leadership, org-design, management, frameworks, microsoft-relevant]
sources: ["https://www.lennysnewsletter.com/p/slack-founder-stewart-butterfield"]
related: ["../podcasts/lenny-stewart-butterfield-slack.md", "../entities/stewart-butterfield.md"]
---

# Hyper-Realistic Work-Like Activities

---

## Definition

A term coined by Stewart Butterfield (and attributed to Fareed, a Slack colleague) for **work that is superficially indistinguishable from real work but produces no value**.

People are sitting in a conference room. Something is being projected. Everyone is talking about it. This is exactly what work looks like. But the meeting is to preview the deck that will be shown at the bigger meeting to get feedback on the slides. Zero net value is being created.

HRWLAs are:
- Called in confidence by well-intentioned, non-evil, non-stupid people
- Indistinguishable from valuable work from the outside
- The natural output of an organization that has more headcount than it has **known valuable work to do**

---

## The Root Cause: Known Valuable Work Supply/Demand

The underlying dynamic is a supply/demand mismatch that develops predictably as organizations scale.

**Known Valuable Work (KVW)**: Work where you simultaneously know (a) what to do, and (b) that it's valuable. At the start of any company or project, KVW is abundant:
- Open a bank account. Obvious. Definitely valuable.
- Create a users table. Obvious. Definitely valuable.
- Write the homepage copy. Obvious. Definitely valuable.

Everyone shows up, has 10 things on their list, every one of them is clearly worth doing, and they do them.

**The mismatch develops**: As time passes, the obvious KVW gets done. Meanwhile, headcount increases — every PM wants a junior PM, every risk & compliance person identifies more risks requiring more compliance people. The supply of obvious KVW shrinks; the demand for work to do grows. The gap fills with HRWLAs.

People aren't doing HRWLAs because they're lazy or evil. They're doing them because:
1. They need to be seen as contributing
2. They're rational actors: headcount under you correlates with salary, authority, and career trajectory
3. No one has explicitly told them what the KVW is, so they fill the void with what looks like work

---

## Parkinson's Law

From a 1955 Economist essay by C. Northcote Parkinson: *Work expands to fill the time available for its completion.*

In the org context: the Royal Navy example. As capital ships decreased and sailors decreased, the number of administrators *increased*. The chart shape is the same in every large organization: headcount grows independently of the work supply.

The PM version: "I need to hire someone. They'll do the product management, and I'll do strategy." This is not cynical — every PM genuinely believes the work exists for the hire. But if you multiply this by 17 PMs, you get 17 junior PMs doing product management and 17 senior PMs doing what exactly? The "strategy" work has a much smaller KVW supply than assumed.

---

## The Slack Threads Example (Perfect Case Study)

A product manager re-introduced pre-populating thread reply boxes with @[previous_poster] — something Butterfield had removed. It came back backed by A/B test data showing threads were **2.17 messages long** with the feature vs. **2.14 without**.

To generate this finding, the organization had to:
- Design and implement feature flags
- Write instrumentation code
- Create database tables to log events
- Build queries against the data
- Create dashboard visualizations
- Prepare a slide deck
- Send calendar invites (and reschedule when someone couldn't make it)
- Hold the meeting

This is thousands of person-hours. The maximum possible value from having @[previous_poster] in the reply box: essentially zero. The statistical finding itself was arguably outside the bounds of confidence. The analysis cost more than the maximum possible benefit — **guaranteed loser**.

It's also not obvious in the moment that this is an HRWLA. Everyone involved thought they were doing rigorous product development. The process had all the hallmarks of good process: data, A/B testing, analysis, review. It was HRWLA performed with complete sincerity.

---

## Why It's Hard to Stop

HRWLAs are "superficially identical to work." Board members do them. Executives do them. The further you are from having full context, full information, and decision-making authority — the easier it is to get trapped.

The meeting to preview the deck for the big meeting is indistinguishable (from outside the room) from the big meeting itself. Both look like "a meeting about the product roadmap."

The A/B test with marginal statistical significance is indistinguishable (from outside the room) from an A/B test that will actually change a major decision.

---

## The Leader's Responsibility

The solution is not to chide people for doing HRWLAs ("you're all wasting time on this thing"). That implies they're dumb, which they're not. **The responsibility lies with the leader**:

1. **Ensure sufficient supply of KVW**: The leader's job is to create clarity around what the priorities are — explicit enough that everyone in the organization can distinguish between "this is known valuable work" and "this is filling a gap."

2. **Say no explicitly upfront**: Before the HRWLA meeting gets called, the right feature or initiative should already be so clearly scoped and prioritized that there's no ambiguity driving the meeting.

3. **The inverse**: If HRWLAs are proliferating, it's not a team discipline problem — it's a KVW supply problem. Ask: have we made clear enough what the most important work is? Is there actually enough of it?

---

## Examples in the Wild

- Quarterly business reviews that review metrics everyone already knows without making any decisions
- "Alignment meetings" where stakeholders with no decision rights discuss a decision that's already been made
- Spec reviews for features that aren't actually being built yet
- A/B tests of features that couldn't move the needle enough to justify the test overhead
- Team offsites with no concrete deliverables
- Decks to explain a decision that was already implemented

In each case: people sitting in rooms, something projected on a screen, everyone talking about it. Looks exactly like work.

---

## PM Application

For a Senior Director of PM at Microsoft:

1. **HRWLA audit of your own calendar**: How many meetings in the past two weeks were called to review something that either (a) had already been decided, (b) had no decision outcome, or (c) were previews of other meetings? This number tells you something about KVW clarity on your team.

2. **KVW clarity as a leadership output**: Your most important contribution is ensuring your teams have clear enough priorities that they don't have to generate HRWLAs to stay visible. Ambiguous strategy is the petri dish for HRWLAs. Explicit "these are the three things that matter" cuts the supply.

3. **The HRWLA test for feature analysis**: Before commissioning a user research study, A/B test, or analysis project, ask: what decision will this change? If the answer is "we'll learn something interesting" or "it validates what we're already doing," it's probably an HRWLA. If the answer is "if the result is X, we'll do A; if it's Y, we'll do B" — that's real work.

4. **Parkinson's Law as a hiring philosophy**: Every PM you hire will generate demand for another PM hire. Before adding headcount, ask whether there's genuinely enough KVW to fill both roles, or whether the new role will fill with HRWLAs. Butterfield's version: "What would that person do?" If the answer is "strategy" while the existing person does "product management" — that's the tell.

5. **Microsoft at scale**: Large organizations like Microsoft have more Parkinson's Law risk than small ones — more veto points, more coordination overhead, more people whose job is to review rather than do. The Senior Director level is particularly susceptible because it's far enough from the work that the HRWLAs don't feel fake. Counter it by staying close enough to the actual product and user that you can tell KVW from HRWLA by feel.

---

## Sources

- [Slack Founder: Mental Models for Building Products People Love](../podcasts/lenny-stewart-butterfield-slack.md) (Stewart Butterfield, 2025-11-20)
