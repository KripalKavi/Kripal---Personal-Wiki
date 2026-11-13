---
title: "Bring Your Own Tokens (BYOT)"
type: concept
date_added: 2026-05-27
tags:
  - ai
  - product-strategy
  - saas
  - pricing
  - frameworks
  - microsoft-relevant
sources:
  - https://www.lennysnewsletter.com/p/the-ai-paradox-dan-shipper
related:
  - ../podcasts/lenny-dan-shipper-ai-paradox.md
  - ../entities/dan-shipper.md
  - ../entities/every.md
  - ../concepts/automation-is-a-lie.md
  - ../concepts/super-agent.md
  - ../concepts/harness-as-moat.md
  - ../concepts/forward-deployed-engineer.md
  - ../concepts/malleable-software.md
---

# Bring Your Own Tokens (BYOT)

## Definition

**Bring Your Own Tokens** is a SaaS economic model in which the customer supplies the inference budget for AI features inside a vendor's app — typically by attaching their own model-provider key (OpenAI, Anthropic, Azure OpenAI) or by accessing the SaaS via their agent (Codex, Cowork, Claude Code) which spends *their* tokens. The SaaS vendor stops paying for inference; the user supplies it.

Dan Shipper's verbatim framing (Lenny's, 2026-05-24):

> "When I run the agent on that website, I'm using my tokens. I'm not using the vendor's tokens, I'm not using the app's tokens. ... For Proof, for anyone who uses it, I don't pay for tokens because they bring their AI to Proof. And so it changes what you build as a SaaS company and you build it now for both humans and agents to use at the same time, and it changes your margins back to, well, I don't really have to pay for tokens anymore because the user's going to bring AI."

Counterintuitive headline: **BYOT improves SaaS vendor margins** rather than cannibalizing them. The vendor keeps the workflow, integrations, and human-in-loop value — the high-margin substrate — and offloads inference, which is becoming commodity.

> "I would buy SaaS stocks right now. I think the SaaS apocalypse is dumb, and SaaS stocks will be up majorly in the next couple years. Not investment advice, but I would buy SaaS stocks."

## Why It Matters

There are two competing macro stories for SaaS in the AI era:

- **SaaSpocalypse** (dominant 2024-2025 take): AI commoditizes vertical SaaS; customers replace per-seat tools with general-purpose agents; SaaS revenue compresses.
- **SaaS-amplification** (Shipper's take): AI changes *what customers pay SaaS for.* They stop paying for inference; they keep paying for the SaaS layer (workflow, integration, identity, permissions, persistence, the maintained substrate). BYOT formalizes the split.

Shipper's claim is stronger than just "SaaS survives" — it's that *demand for SaaS goes up* under BYOT:

> "What agents do is increase the number of users of SaaS, not get rid of it. And so I think SaaS companies are going to see an insane spike in the amount of demand that they have, because there's going to be tons of agents using these products at a very high volume."

If the amplification story is right, the economic implications invert:

- SaaS vendor COGS drops (no more inference markup risk; no more cap-table exposure to model price changes).
- Customer's total spend may rise, but it splits into "SaaS subscription" (margin-rich) + "inference" (paid directly to model provider).
- The vendor's margin profile *improves* because the part they keep is the high-margin part.
- The vendor's competitive position *strengthens* because they are no longer exposed to model-pricing volatility — the customer absorbs it.

This is consistent with Max Schoening's argument that *"the thing you pay for as a service is the maintenance and a bunch of specialists thinking really hard about a problem"* — see [Malleable Software](malleable-software.md). Inference is not the service; the substrate is.

## How BYOT Actually Manifests

Shipper distinguishes the *attached-key* form ("set your OpenAI key in settings") from the *agent-mediated* form ("the user opens the app inside their Codex/Cowork/Claude Code session"). Both produce the BYOT margin effect; the agent-mediated form is the more interesting one because it's *unavoidable* once users live in agent consoles.

The implication for what you build:

> "Once you have a coding agent on your computer that can build anything, it's actually really good for any kind of work you want to do. And people started just hacking Claude Code, essentially, to do all of their work."

> "You actually don't really need to think about having an AI surface that's primarily going to be the thing that users use in the sense that you don't need to build an agent necessarily into your product."

The vendor is freed from the "build an AI feature" race because the user already has an AI feature — their agent. The vendor's job becomes *be a good agent target.*

What "agent-friendly" means concretely:

- Stable, well-documented HTML for the agent to read.
- A CLI / API surface that's coherent with the GUI (Shipper: *"everyone's got a CLI now, you want to make the HTML really usable. You want to make sure that anything that happens in the CLI shows up for the user immediately"*).
- Approval flows / inbox / undo for the human-in-loop side of hybrid usage.
- Infrastructure that can absorb agent-rate traffic (an agent can make a billion requests in three seconds).

## Examples / Evidence

- **Proof (Every's open-source markdown editor)** — the worked example. Users bring their AI; Proof pays no token costs; the SaaS layer is the editor + integration + sync.
- **Cursor's enterprise tier** has supported customer-provided keys for major models since 2024. Cursor's margin trajectory has been visible in its ARR.
- **Claude Code, Codex, OpenCode, and Gemini CLI** all support multiple backends with user-provided keys; the harness wraps multiple model providers (see [Harness as Moat](harness-as-moat.md)).
- **Many vertical SaaS apps (2025-2026)** that initially priced "AI features included" walked back to "AI features as add-on" or "bring your own key" to manage margin volatility from inference price swings.
- **Microsoft's Azure AI Foundry positioning** toward enterprise customers who want choice over model selection is the BYOT-shaped offering at the platform layer — but M365 Copilot does not yet ship BYOT broadly.

## What BYOT Doesn't Mean

- It doesn't mean the SaaS vendor exits the inference business. Many will offer "use ours by default, bring your own if you prefer."
- It doesn't mean SaaS pricing drops. It often *rises*, because the SaaS subscription now reflects the workflow value cleanly without inference noise.
- It doesn't mean customer cost drops. Customers may pay more total when they include their direct inference spend — but they pay for it transparently.
- It doesn't mean small SaaS startups win. Larger players with the substrate and integration lead compound advantage under BYOT because that's what the customer is paying them for.
- It doesn't mean SaaS vendors stop investing in AI features. They still need to be a good agent target, which is a real engineering investment. It just *isn't* "ship a chatbot."

## PM Application

For a Senior Director of PM at Microsoft:

1. **Decide explicitly whether M365 Copilot supports BYOT for enterprise customers, and on what timeline.** This is a Microsoft-specific tension: M365 sells the SaaS substrate *and* the inference (via Azure OpenAI and increasingly other providers). Internal incentives push against BYOT because it cannibalizes Azure-attached inference. External pressure for BYOT will come — Cursor, Notion, and others already enable it. The right answer is to let the customer choose, then capture them on whichever rail they prefer.

2. **Re-instrument Copilot margin reporting.** If BYOT becomes available, you want to see margin per seat *with* inference cost broken out, so the workflow-value margin is legible separately from the inference markup. This is the input metric for the strategic call in (1).

3. **Use the Azure rail to capture BYOT customers.** A customer who chooses BYOT from M365 Copilot doesn't have to escape Microsoft — they can route inference through Azure OpenAI or Azure-hosted Anthropic. Total Microsoft economics can stay strong even if the M365 line item gets cleaner. This requires aligned packaging across M365 and Azure orgs.

4. **Apply the same lens to GitHub Copilot.** GitHub's enterprise tier already offers some model choice; pushing BYOT further is consistent with [Harness as Moat](harness-as-moat.md). Customer's keys, customer's models — workspace, integrations, policies stay GitHub.

5. **Beware "we make our margin on inference" framing inside Microsoft.** That framing is correct *today* and dangerous as a *strategy.* Inference is converging to commodity; the substrate is not. Margin should compound where the moat is.

6. **Engineer M365 apps to be excellent agent targets, not chatbot hosts.** Shipper's Proof example shows the design discipline: stable HTML, coherent CLI/GUI, approval flows for hybrid use, infrastructure for agent-rate traffic. Word, Excel, Outlook, Teams, and OneNote should each be ranked on agent-target quality. That ranking should drive engineering investment more than ranking on chatbot UX.

7. **Plan for the SaaS demand spike, not the SaaS collapse.** Shipper expects an "insane spike" in SaaS demand from agents at high volume. M365 capacity, throttling, identity, and audit infrastructure should be planned against that scenario, not against the eliminationist scenario.

## Connection to Other Concepts

- **[Automation Is a Lie](automation-is-a-lie.md)** — both ideas argue the value isn't in the model; it's in the human-and-workflow scaffolding around it.
- **[Harness as Moat](harness-as-moat.md)** — BYOT is the pricing-side expression of harness-as-moat. If the harness is the moat, then sell the harness and let the customer buy the model.
- **[Super-Agent](super-agent.md)** — the company super-agent and the BYOT consumer model both push inference cost out of the vendor stack and onto the user/customer side.
- **[Malleable Software](malleable-software.md)** — *"The thing you pay for as a service is the maintenance and a bunch of specialists thinking really hard about a problem."* Schoening's frame and BYOT economics are the same insight from two angles.
- **[Forward-Deployed Engineer](forward-deployed-engineer.md)** — FDEs configure the substrate; BYOT prices it. Both treat inference as the commodity layer and the integration/workflow as the value layer.

## Sources

- [The AI Paradox — Dan Shipper on Lenny's Podcast](../podcasts/lenny-dan-shipper-ai-paradox.md) — 2026-05-24, primary articulation with Proof as worked example

## Related

- [Automation Is a Lie](automation-is-a-lie.md)
- [Super-Agent](super-agent.md)
- [Harness as Moat](harness-as-moat.md)
- [Forward-Deployed Engineer](forward-deployed-engineer.md)
- [Malleable Software](malleable-software.md)
