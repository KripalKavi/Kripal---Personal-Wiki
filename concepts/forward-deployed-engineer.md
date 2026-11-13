---
title: "Forward-Deployed Engineer"
type: concept
date_added: 2026-05-27
tags:
  - ai
  - org-design
  - agentic-ai
  - enterprise
  - career
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
  - ../concepts/builder-vs-information-mover.md
  - ../concepts/cultivating-agency.md
  - ../concepts/harness-as-moat.md
---

# Forward-Deployed Engineer (FDE)

## Definition

A **forward-deployed engineer** is an engineer embedded inside the customer's organization (or, increasingly, in the same role internally) to operate and customize an agent so it works well in that specific context. Historically a Palantir term; in the AI era, the role becomes the most essential new hire because *every agent needs a human who cares about it.*

Dan Shipper's verbatim framing (Lenny's, 2026-05-24):

> "The whole forward-deployed engineer concept I think is for real and it comes out of every agent needs a human. You go to the big model companies, they have these agents that run internally, they have teams of people that run these agents and I don't think those teams are going away. The models are going to get more powerful, the agents are going to get more powerful and the number of agents is going to grow, but people are still going to manage them."

The role is structural, not transitional. Shipper expects it to grow as models and agents grow.

## Why It Matters

The role exists precisely *because* [Automation Is a Lie](automation-is-a-lie.md). If agents were drop-in, FDEs would be unnecessary. They aren't, so FDEs are the unlock. Three properties of agent work make the role structural:

1. **Domain logic is intrinsically local.** Compliance regimes, internal vocabularies, naming conventions, approval matrices, integration touchpoints — none of these are in the model. Someone has to bring them.
2. **The integration surface is unbounded.** Every customer has a different CRM, a different ticketing system, a different chat tool, a different data warehouse. The integration is the product; the agent is the easy part.
3. **Evals must be customer-specific.** Generic benchmarks don't predict performance on the customer's data. FDEs build the evals (see [AI Evals](ai-evals.md)) that prove the agent works for that workload.

Shipper insists the framing isn't "babysitting":

> "I would sort of split it into less babysitting agents and more your forward deployed team is trying to build a whole system that makes it so that people who have less knowledge can use that system without doing something dumb. And that's like a really interesting engineering challenge."

The FDE is *building infrastructure* that lets a non-technical workforce safely use agents — not playing whack-a-mole on agent errors.

## The Canonical Examples

- **Nitesh at Every.** Runs **Claudy** — Every's company-wide consulting super-agent. Shipper:

> "Nitesh, who fits this, he's an AI engineer and he fits this sort of forward deployed category and he's on our team. He spends most of his time actually talking to one of our agents in Slack. We have an agent internally called Claudy, which runs our whole consulting practice and he spends a lot of time in Slack. There is code and he is using Claude Code and other things like that, but a lot of it is just talking to it and being like, 'Why did you do this dumb thing? Let's fix that.'"

The job is half engineering, half operations, half teaching. The role attracts a specific kind of engineer: *"there's certain kinds of engineers that I think love that and love having their hands on the latest thing and also love making this being that's in a workspace and it looks a bit different than more traditional building."*

- **The big-lab data-science FDE team.** Shipper:

> "The way that it works inside of the big model companies, for example, at least one of them has literally a data science bot that every single person in the org can query that is hooked up to their data warehouse that knows who's who so that it knows at the warehouse level who has permission to access what. And so all of the basic questions, because there's a team that sets up this bot, all of the basic questions that people might want to ask that it sometimes that might get wrong, that they're constantly making sure it's getting it right. And so the data science team doesn't have to answer all the bullshit questions because there's another team building an agent that is set up to do that really well. But if the team didn't exist, the data scientists would hate their lives."

This is the *internal* FDE pattern — a team whose product is the company's internal super-agent.

- **Anthropic and OpenAI internal agent teams.** Both run internal agents at scale with named teams whose job is keeping them working. Shipper expects those teams to grow, not shrink, as models improve.

- **Pete on OpenClaw.** Triages thousands of agent-generated PRs per day, merges ~1,000. The FDE-equivalent at the open-source layer.

## What FDEs Actually Do

- Map the customer's workflow to the agent's capability surface — what should the agent touch, what should it never touch.
- Write the domain-specific prompts, tools, and integrations the agent needs.
- Build customer-specific evals against the customer's data.
- Tune permission boundaries, audit logging, and human-in-loop checkpoints.
- Onboard customer staff to the new agent-augmented workflow.
- Garden the super-agent in Slack — answer questions, fix dumb behaviors, extend capabilities, push back on the model.
- Hand back observability and feedback infrastructure the customer will own long-term.

Notice that none of this is *"deploy the model."* The model is the cheap part.

## PM Application

For a Senior Director of PM at Microsoft:

1. **Invest in the customization surface as a product, not a deployment cost.** Copilot Studio, Power Platform, Graph extensibility, agent SDKs, and the eval tooling around them are the *product* that FDEs build *with.* If those surfaces are weak, every FDE engagement is slower, more expensive, and less repeatable. The leverage on FDE productivity is the surface — a PM problem, not a services problem.

2. **Resource the FDE motion as a strategic asset, not a cost center.** Microsoft has historically split this between consulting/services and product engineering. The Shipper framing argues for a middle category: a *product-aware FDE org* whose feedback loop directly drives product investment. Anthropic and Palantir both run this way; Microsoft can.

3. **Track FDE deployment as a leading indicator of expansion.** The number of customer deployments with an embedded engineer (Microsoft, partner, or customer-paid) is a stronger predictor of seat expansion than any feature signal. Instrument it.

4. **Build the FDE career ladder.** Not a band-3 contractor job. A senior, deep-context, multi-discipline engineer who needs a promotion path, equity participation, and visible internal status. The talent market is competitive — losing them to Anthropic or Palantir is a real cost. Agency-bearing engineers self-select into FDE roles; see [Cultivating Agency](cultivating-agency.md).

5. **Frame FDE work as "building the system, not babysitting the agent."** Shipper's exact reframe matters for hiring, retention, and internal status. The FDE who thinks of themselves as a glorified prompt engineer burns out; the FDE who thinks of themselves as building the infrastructure that lets the rest of the company safely use AI does not.

6. **For the super-agent in Teams motion, FDE is the named deliverable.** Microsoft (or partner) FDE engagements should ship the customer's super-agent — not just integration packages. The super-agent is the visible product of the FDE engagement. See [Super-Agent](super-agent.md).

7. **Beware "the agent will sell itself" pitches internally.** If a Copilot product proposal claims minimal in-customer integration work, scrutinize the model of adoption. The empirical pattern says the integration is the work. Sales motions and pricing should reflect that, not paper over it.

## Connection to Other Concepts

- **[Automation Is a Lie](automation-is-a-lie.md)** — the FDE role is the operational form of automation-is-a-lie. If the lie were true, FDEs wouldn't exist.
- **[Super-Agent](super-agent.md)** — the FDE is the named human who cares about the super-agent. The two concepts are co-defining.
- **[Builder vs. Information Mover](builder-vs-information-mover.md)** — FDE is the canonical builder role for the enterprise. They build the agent-customer fit, hands-on.
- **[Harness as Moat](harness-as-moat.md)** — FDEs are the human side of harness defensibility. They tune the harness for each customer; that tuning is what survives model swaps.
- **[Cultivating Agency](cultivating-agency.md)** — FDEs are agency-maximalists by selection. The role rewards initiative and judgment, not process discipline.

## Sources

- [The AI Paradox — Dan Shipper on Lenny's Podcast](../podcasts/lenny-dan-shipper-ai-paradox.md) — 2026-05-24, primary articulation; Nitesh and Claudy at Every as named examples; "building the system, not babysitting" reframe

## Related

- [Automation Is a Lie](automation-is-a-lie.md) — the why
- [Super-Agent](super-agent.md) — what the FDE gardens
- [Bring Your Own Tokens](bring-your-own-tokens.md) — the economic counterpart
- [Builder vs. Information Mover](builder-vs-information-mover.md) — the career-shape counterpart
- [Harness as Moat](harness-as-moat.md) — what FDEs are tuning
