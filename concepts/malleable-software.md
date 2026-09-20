---
title: "Malleable Software"
type: concept
date_added: 2026-05-15
tags: [product-strategy, ai, design, agentic-ai, microsoft-relevant]
sources: ["https://www.lennysnewsletter.com/p/why-cultivating-agency-matters-more", "https://fs.blog/knowledge-project-podcast/tobi-lutke-3/"]
related: ["../podcasts/lenny-max-schoening-agency-over-skills.md", "../podcasts/knowledge-project-tobi-lutke-ai-agents-judgment.md", "../entities/max-schoening.md", "../entities/notion.md", "../entities/shopify.md", "../concepts/harness-as-moat.md", "../concepts/cultivating-agency.md", "../essays/lenny-claire-vo-openclaw-personal-ai-agent.md"]
---

# Malleable Software

## Definition

**Malleable software** is software designed to work closer to the interest of the people that use it than the interest of the corporation that makes it. It can be shaped, customized, recomposed, and extended by its users — not as a power-user escape hatch, but as a first-class design value.

[Max Schoening](../entities/max-schoening.md) (Notion) has held this belief for years, since well before the AI wave:

> "Malleable software is the idea that software works closer to the interest of the people that use it than the interest of the corporation that makes it... I don't want to use software that is specifically just designed by the ivory tower in Cupertino."

The contrast he draws is physical:

> "Imagine you lived in an environment where you do not get to rearrange your living room and the kitchen has to be exactly set up the way that someone else decided. We would not take that. But that is kind of the world that we have in software right now where we have this world of apps, and apps are this very — every layer is glued together — of the user interface, the data ownership and so on. And the moment you're like, 'this is a really great app, but I just want to change a little bit,' that is usually not possible."

---

## The Two Failure Modes Malleable Software Avoids

1. **The ivory-tower app** (Schoening's main target): every layer glued together, vendor decides, user gets no recomposition. Most apps. Most M365 surfaces. Most SaaS.

2. **The "build your own everything"** counter-extreme: run your own Linux distro. *"You realize, 'I like the malleability, but I also have other things to do, and I don't always want to start from scratch and figure out why the trackpad doesn't work.'"* Personal-AI-agent maximalism risks falling here. See [OpenClaw](../essays/lenny-claire-vo-openclaw-personal-ai-agent.md).

The right point is in between: **communal, malleable platforms.** The user shapes their own tools but inherits collaborative infrastructure, real-time sync, security, and updates from a maintained substrate.

---

## Why AI Is the Trigger

Malleable software was Schoening's belief for a decade, but it was "always slightly too hard." AI is the unlock:

> "Now you're making your own tools maybe for podcast recording, for prepping for shows or whatever. There's a myriad examples and people are awakening to this idea of: 'Oh, I can just make tools.'"

When making a tool drops from "spec, hire engineer, integrate" to "describe what you want, get a working version in five minutes," malleability becomes a *user expectation*, not a power-user perk. Schoening points to Geoffrey Litt's work at Ink & Switch as the canonical research thread.

---

## The Communal-Tools Requirement

Schoening pushes against personal-AI-agent isolationism:

> "It has to be built on top of a platform or an operating system that encourages this, because otherwise we're just doing individual little tools, everybody has their own. And I like communal tools."

This is the strategic insight: malleable software needs a substrate. The substrate is the moat. Notion positions itself as that substrate (*"I think of Notion as an operating system"*). Connected workspace + agents-can-roam + user-can-shape = malleable platform.

Lütke describes a complementary organizational version: an AI-shaped operating system that can fulfill wishes and evolve through conversation, plus Shopify's River as a shared AI colleague. The substrate is useful when it is both malleable and communal—individual workflows can change without every person having to maintain an isolated system.

This is the natural overlap with [Harness as Moat](../concepts/harness-as-moat.md): the harness *is* the substrate that enables malleability while preserving communal infrastructure.

---

## Physical Analogs (Schoening's References)

- **Christopher Alexander, *The Timeless Way of Building*** — buildings that adapt to their inhabitants over time.
- **Stewart Brand, *How Buildings Learn*** — the best homes are usually not built by architects; they're built by an architect-shell that adapts over decades to actual use.
- **Dieter Rams** (the video pinned to Schoening's Twitter profile) — *"design should be first useful and then beautiful."* The piece is in a museum if it isn't useful. *"For that cabinet, he says, 'it is neither orderly nor properly chaotic.'"* Malleable software's bar: useful enough that change is invited, not forbidden.
- **Tools of Conviviality** ([Ivan Illich](../books/illich-tools-of-conviviality.md)) — the deep canonical text. Convivial tools amplify human autonomy; industrial-scale tools destroy it.

---

## SaaS Apocalypse Counterargument

Malleable software *doesn't* mean SaaS dies. Schoening explicitly rejects the SaaSpocalypse:

> "I've tried rebuilding Notion in a weekend for myself just to push at the edges of frustrating things. I don't think people want that. People just want to go to Costco and have the steak in styrofoam packaging and pretend that it wasn't hunting or an animal in the first place. Software is a garden — you need to tend to it. The thing you pay for as a service is the maintenance and a bunch of specialists thinking really hard about a problem."

The malleable-software future is **more general SaaS, not less.** Tools become more general-purpose (closer to the '90s — WordProcessor, spreadsheet, FileMaker Pro) but stay "as a service." Specialized tools survive on the edges where someone goes the extra mile. Anthropic uses Slack despite being uniquely capable of rebuilding it — *"nobody wants to rebuild a tool like Slack."*

**Dan Shipper makes the same argument from the pricing side.** On Lenny's, 2026-05-24, he predicts SaaS thrives — *"buy SaaS stocks right now"* — because users bringing their own AI tokens into apps *improves* vendor margins. The customer keeps paying for the substrate (maintenance, integration, workflow); they stop paying the vendor for inference. Two senior product leaders (Schoening at Notion, Shipper at Every) converge on the same conclusion from opposite directions. See [Bring Your Own Tokens](../concepts/bring-your-own-tokens.md).

---

## PM Application

For a Senior Director of PM at Microsoft:

1. **Reposition M365 as a malleable platform, not an app suite.** Word, Excel, Outlook, Teams, OneNote — the classic frame is "best-in-class apps." The malleable-software frame is *"the M365 substrate where you make the tools you want."* Copilot Studio, Power Platform, Loop components, and Graph extensibility *are already this* — but they're not narrated this way internally or externally. Tell that story explicitly.

2. **Bet against rigid apps; bet for shaped substrates.** Schoening's framing makes a generational bet: vendors that stay "every-layer-glued-together" lose to platforms that let users shape their software. Microsoft's history is mixed here — VBA was malleable; "modern Office" pulled back; Copilot Studio is opening it again. The strategic question: does the next generation of M365 *invite reshaping* or fight it?

3. **Graph as the convivial substrate.** Ivan Illich's "tools of conviviality" maps directly onto Graph + agent SDKs: a substrate where users (and the agents acting for them) can compose tools that fit their work. Frame Graph this way internally; it changes investment priorities. See [Harness as Moat](../concepts/harness-as-moat.md).

4. **Don't fear the maker class.** Some PMs see user-built tools as a threat (fragmentation, support cost, lost engagement). Schoening's argument: maker culture *strengthens* substrate platforms. Notion users who build their own tools become Notion's deepest users. The defensive PM move is to fragment user agency; the offensive move is to channel it into the substrate.

5. **Beware "users won't customize." They do, when it's easy.** The old assumption that customization is a power-user feature breaks when AI makes customization conversational. Most M365 features still assume non-customization is the default. The default should flip: every Copilot surface should ask, *"how do users shape this for themselves?"*

6. **Connect to user agency.** [Cultivating Agency](../concepts/cultivating-agency.md) and malleable software are the same idea at different layers — agency over your work and agency over your tools. Microsoft can stand for: *we give you a workspace that bends to you, and we give you agents that act on your behalf.* This is a clear, defensible positioning.

---

## Sources

- [Lenny's Podcast — Max Schoening](../podcasts/lenny-max-schoening-agency-over-skills.md) — primary articulation, 2026-05-03
- Ink & Switch malleable-software research (referenced, Geoffrey Litt)
- [Tools of Conviviality](../books/illich-tools-of-conviviality.md) — Ivan Illich
- *The Timeless Way of Building* (Alexander), *How Buildings Learn* (Stewart Brand)

## Related

- [Harness as Moat](../concepts/harness-as-moat.md) — the substrate that enables malleability while preserving communal infrastructure
- [Cultivating Agency](../concepts/cultivating-agency.md) — agency-over-tools is malleable software's user-side counterpart
- [OpenClaw / Claire Vo](../essays/lenny-claire-vo-openclaw-personal-ai-agent.md) — the personal-AI-agent extreme that Schoening considers too isolated
- [Bring Your Own Tokens](../concepts/bring-your-own-tokens.md) — the pricing-side expression of the same insight: pay the vendor for the substrate, not the inference
