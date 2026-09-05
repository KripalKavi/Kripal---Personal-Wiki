---
title: "Notion"
type: entity-company
date_added: 2026-05-15
tags: [product-strategy, ai, productivity, microsoft-relevant]
sources: ["https://www.lennysnewsletter.com/p/why-cultivating-agency-matters-more"]
related: ["../entities/max-schoening.md", "../podcasts/lenny-max-schoening-agency-over-skills.md", "../concepts/tiny-core.md", "../concepts/malleable-software.md", "../concepts/harness-as-moat.md"]
---

# Notion

## What They Do

Productivity software positioned as a **connected workspace** — docs, wikis, databases, projects, and (since 2023) AI all sharing a unified data model. Founded by Ivan Zhao. Started as a website builder; pivoted to document collaboration in 2014. The first version of the editor was infamously rough (*"you couldn't even select between two blocks"*) but the core primitive was right.

In 2026, Notion frames itself less as a doc app and more as an **operating system** for knowledge work — a substrate that AI agents can roam in.

## Growth Story

Key inflection points:
- **2014 pivot**: From website builder to document collaboration — the pivot that defined the company. Caused at least one would-be competitor (Schoening's startup) to lose a term sheet from True Ventures.
- **Blocks + slash commands** became the [Tiny Core](../concepts/tiny-core.md). Every doc element is a block, addressable, composable. Slash-command for inserting any block type. Schoening: *"At Notion, it's the blocks and the slash commands."*
- **Connected workspace**: a decade of patient work integrating docs, databases, projects, comments, wikis under one data model. Was considered "kind of hard to get started" pre-AI.
- **AI assistant (pre-ChatGPT)**: Ivan Zhao and Simon Last shipped the first Notion AI assistant before ChatGPT. Early conviction that this would change everything.
- **Notion AI agent (2026)**: surprisingly successful launch. Schoening, who is his own first critic, said he's *"surprised at how good it is."* External signal: journalist Joanna Stern tweeted *"thanks to Notion AI, I finally understand and use Notion."*
- **AGI-era positioning**: Schoening describes Notion as *"resembling the environment that coding agents are in with Unix"* — i.e., a Unix-shaped substrate for agents.

## Strategic Insights

1. **Connected workspace = Unix for agents.** Schoening's read: agents need context to roam in. Walls between data repositories choke them. Notion's decade of connected-workspace work suddenly became load-bearing for AI-era PMF — patient infrastructure that wasn't obviously valuable until agents needed it. This is the single most important strategic insight for Microsoft: **Graph + M365 is a vastly larger version of the same asset.**

2. **Tiny core discipline pays off across decades.** Notion's blocks primitive was strong enough that a *clearly worse* editor still beat polished alternatives. Schoening's 2014 competitor had markdown folding (now seen in Obsidian) and lost anyway. The lesson: get the core right; everything else is tractable. See [Tiny Core](../concepts/tiny-core.md).

3. **Designers and PMs ship code; the medium is the agent loop.** Notion-internal practice (championed by Schoening): designers prototype AI surfaces in code, not Figma. Reason: *"the static image of a chat is the dead fish"* (Bret Victor). PMs also work in TUIs like Claude Code and Codex. Marketing teams ask designers to reverse-engineer designs back to Figma for assets — Schoening calls this "busy work."

4. **High agency culture is the operating norm.** Schoening: Notion design team has "above-average agency compared to other places I've worked at." Examples: Brian Levin/Lovin recruits aggressively because the org needs it; Eric Lou rewrote his own job to drop PRDs → Figma → prototype-in-code over a year. See [Cultivating Agency](../concepts/cultivating-agency.md).

5. **Token spend is unlimited (for now).** Schoening, as Head of Product, doesn't track which engineers spend the most tokens. *"It is just the wrong thing to optimize for. When something new comes along, it's worth letting people explore."* One Notion PM is the company's #1 token spender. ROI conversations will come in 6–12 months.

6. **Shots on goal + Obviously good.** Two simultaneous principles: ship more experiments, but only ship things that are *obviously good.* Resolved through incremental correctness — iterate in public, not in a cave.

7. **Six automation primitives = consolidation debt.** Notion currently has six different automation primitives (counting agents). Schoening admits this is too many and that consolidation back to a [Naked Robotic Core](../concepts/naked-robotic-core.md) is overdue.

8. **Conference rooms named after objects of taste**: first typewriter, Macintosh, Porsche 911. Deliberate environmental nudge to keep the craft bar high. *"Inevitably when I'm sitting in one of the rooms, nothing I'm doing amounts to this. I got to do better."*

## Why It Matters to Microsoft

Notion competes most directly with Microsoft 365 (OneNote, Loop, Teams docs, SharePoint, Lists). Key strategic implications for Microsoft PMs:

- **The connected-workspace pattern is the playbook.** Microsoft owns the largest connected workspace in the world (Graph + M365). Notion's success at agent-PMF via connected workspace is the strongest evidence that this is the right substrate for AI. The question is whether Microsoft *operates* on it like Notion does or merely possesses it.
- **The agent UX bar is rising fast.** Notion AI agent quality is a real benchmark for Copilot for Microsoft 365.
- **Workspace harness, not model, is where users settle.** Notion can use frontier models from any lab; users stay because of the workspace, not the model. Same is true for Copilot — invest accordingly. See [Harness as Moat](../concepts/harness-as-moat.md).
- **Notion is malleable; Microsoft historically isn't.** Schoening's belief in [Malleable Software](../concepts/malleable-software.md) is a deliberate competitive positioning against rigid enterprise software (read: Microsoft). The defensive move for Microsoft is to make Copilot the layer through which users *make* M365 more malleable to themselves — agent-mediated customization at scale.

## Appearances

- [Why Cultivating Agency Matters More Than Cultivating Skills in the AI Era](../podcasts/lenny-max-schoening-agency-over-skills.md) — Max Schoening, Lenny's Podcast, 2026-05-03

## Key People at Notion (mentioned across sources)

- **Ivan Zhao** — Founder
- **Simon Last** — Co-founder / engineering
- **Max Schoening** — Head of Product
- **Brian Levin/Lovin** — Designer; canonical high-agency example
- **Eric Lou** — PM; example of role-reinvention via building skills
