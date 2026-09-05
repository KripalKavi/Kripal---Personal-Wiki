---
title: "Every"
type: entity-company
date_added: 2026-05-27
tags:
  - ai
  - media
  - agentic-ai
  - product-strategy
sources:
  - https://every.to
  - https://www.lennysnewsletter.com/p/the-ai-paradox-dan-shipper
related:
  - ../entities/dan-shipper.md
  - ../podcasts/lenny-dan-shipper-ai-paradox.md
  - ../concepts/automation-is-a-lie.md
  - ../concepts/super-agent.md
  - ../concepts/forward-deployed-engineer.md
  - ../concepts/bring-your-own-tokens.md
---

## What They Do

Brooklyn-based media + software company founded and run by [Dan Shipper](../entities/dan-shipper.md). Publishes essays on tech, business, and AI's effect on knowledge work. Runs a portfolio of AI tools, each instantiating a specific thesis about how AI changes work. The publication-plus-tools model treats writing and software as the same product motion: essays surface patterns; tools embody them.

## Team & Scale

- ~30 employees as of May 2026 (doubled from 15 a year earlier)
- All employees are AI early adopters: engineers, designers, writers, editors, salespeople, customer service. Shipper screens for it.
- Runs six internal software products as of mid-2026 (up from two or three a year earlier).
- Located in Brooklyn — Shipper's framing: *"the edge of AI is wherever AI meets a real human doing something,"* not San Francisco.

## Internal AI Products & Workflows

- **Proof** — open-source markdown editor. Shipper's daily writing surface. Used inside Codex's in-app browser; the worked example for [Bring Your Own Tokens](../concepts/bring-your-own-tokens.md) because users supply their own AI tokens when they bring an agent to Proof. *"For Proof, I don't pay for tokens because they bring their AI to Proof."*
- **Spiral** — Every's writing app. Run by **Marcus** (PM by background, ex-Axios writing product, "lightly technical"). The canonical "PMs thrive" example in this episode.
- **Cora** — productivity tool (writing/inbox area).
- **Lex** — AI-first writing tool.
- **Quora** — Every's internal email agent. Gathers Shipper's email, renders a page, he monologues responses; Codex executes. Got him to inbox zero for 10 days straight at time of recording.
- **Hosted OpenClaw** — was on waitlist; *paused* because too hard to maintain. Strong evidence for [Automation Is a Lie](../concepts/automation-is-a-lie.md): even the company built specifically to operate agents at the frontier could not run the personal-agent harness as a hosted product reliably. Triggered Shipper's flip from personal-agent → super-agent architecture.
- **Claudy** — Every's internal company-wide super-agent in Slack. Runs Every's entire consulting practice. Owned by Nitesh (the forward-deployed engineer). See [Super-Agent](../concepts/super-agent.md) and [Forward-Deployed Engineer](../concepts/forward-deployed-engineer.md).
- **Quarterly planning via Notion Agents (end of 2025)** — every team member talked to a Notion Agent, which asked about prior year, goals, metrics, pushed back, then synthesized into a strategy report per team. *"I got these incredibly good AI generated strategy reports or quarterly plans for each part of each team."*

## Named People Worth Tracking

- **Marcus** — runs Spiral. Lightly technical PM, ex-Axios. Canonical "PMs thrive" exemplar.
- **Nitesh** — AI engineer / forward-deployed engineer. Runs Claudy. Spends most of his time in Slack talking to the agent.
- **Brandon Gell** — COO. Coined *"computer errands"* (the personal-agent split from work-agent territory).
- **Pete** — runs OpenClaw. Receives thousands of pull requests a day; spins up 50,000 Codex instances to triage; merges 1,000. Operational example of the new shape of work under agent volume.

## Strategic Insights

- **"Living lab" as a content moat.** Most AI commentary is forecast; Every's is observation. The credibility differential compounds, and is why Shipper gets early access to model releases — *"because of our role reviewing models and being a little bit of a pacemaker in AI, we get access to stuff before it comes out."*
- **Tools-as-thesis.** Each Every product instantiates a specific argument about AI-changed work — Spiral for repeatable writing, Cora for inbox, Lex for drafting, Proof for both-human-and-agent editing.
- **30 people > N people, at agent leverage.** Every is the existence proof for Shipper's "more humans, more work, more output" thesis. Doubled headcount, doubled or tripled product count, expanded scope.
- **Nontechnical agent adoption is the real signal.** Every's non-engineers using Claude Code / Codex day-to-day is the leading indicator that the agent console is escaping the developer audience.
- **Public flips.** Shipper announced this episode's super-agent flip publicly. The willingness to update — and reason about *why* — in public is part of Every's editorial brand.

## Appearances

- [The AI Paradox — Dan Shipper on Lenny's](../podcasts/lenny-dan-shipper-ai-paradox.md) — 2026-05-24

## Why It Matters for Microsoft

Every is the closest available "control group" for how a maximally AI-forward small org actually operates. When the next round of M365 Copilot adoption studies lands, Every's lived patterns (super-agent in Slack + Codex/Cowork for individual work + FDE-driven gardening + BYOT for SaaS) are the realistic ceiling for what customer orgs will look like a year out. Designing M365 for that ceiling — not for "Copilot replaces the engineer / accountant / writer" — is the strategic posture.
