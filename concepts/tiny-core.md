---
title: "Tiny Core"
type: concept
date_added: 2026-05-15
tags: [product-strategy, design, frameworks, microsoft-relevant]
sources: ["https://www.lennysnewsletter.com/p/why-cultivating-agency-matters-more"]
related: ["../podcasts/lenny-max-schoening-agency-over-skills.md", "../entities/max-schoening.md", "../concepts/naked-robotic-core.md", "../concepts/utility-curves.md", "../concepts/we-dont-sell-saddles-here.md"]
---

# Tiny Core

## Definition

Every great product wins through **one tiny, exceptionally good core mechanic** — not through feature breadth. The tiny core is the single primitive that, once experienced, makes the rest of the product feel inevitable. Failing products try to compensate for a missing tiny core by adding features. It never works.

[Max Schoening](../entities/max-schoening.md) (Head of Product, Notion):

> "All the great products have something tiny that is a superpower, one tiny core that is so exceptionally good... One of the biggest pitfalls is if you get into the loop of, if I just add one more thing to the product, it'll be finally great. That never works."

---

## Why It Matters

Most product debates are downstream of whether the tiny core is right. If it is, everything else is tractable — UI can be ugly, onboarding can be confusing, feature set can be thin. Notion's first editor in 2014 was famously rough (Schoening: *"you couldn't even select between two blocks"*) and it still won, because **blocks were the right tiny core.**

If the tiny core is wrong, no amount of feature-adding rescues the product. Schoening's confession from his 2014 Notion competitor: he and his team polished the editing experience (markdown folding, what's now in Obsidian) for months before realizing they were *"working diligently on the wrong thing for way too long."*

The implication for product reviews: the meaningful question is rarely *"is this feature good?"* It's *"is the core right?"* If yes, ship roughly and iterate. If no, no feature will save you.

---

## Schoening's Catalog of Tiny Cores

- **iPhone**: multitouch
- **GitHub**: the pull request — *"this idea that anyone can suggest something to you and you see it"*
- **Notion**: blocks + slash commands
- **Heroku**: `git push heroku master` — *"this very simple one-liner that went from the thing on my computer, now I have a URL. That's so intoxicating that everything else flows from there."*
- **Dropbox**: the menu-bar icon for sync — *"it was so good at syncing that you could even use it as a symbol for 'do I have internet or not?' because it was better at figuring out whether you had an internet connection than your Mac itself."* And then *"for years they've tried to increase the surface area. I kept thinking — no, no, no, push it back. I don't want more. This is the only job I want from you."*
- **Figma**: seamless blend of real-time collaboration and not
- **Snapchat**: disappearing photos
- **AirPods** (Schoening adds): not the first Bluetooth headphones — *"they were the first that connected and so on. They weren't the first MP3 player. You just got to do it right."* This is the *"be right, not first"* principle.

---

## The Feature-Creep Anti-Pattern

> "If I just add one more thing to the product, it'll be finally great. That never works."

Schoening's lived failure mode: when the core isn't landing, the natural urge is to *"keep adding yet another feature: okay, is it good now? Is it good now?"* The death spiral is feature-by-feature interrogation of a fundamentally weak core.

The correct response when a core isn't working: don't give up on the *idea* of having a tight core — change the core. Don't paper it over with features.

---

## Tiny Core for AI Products

The implicit prescription for the current AI product wave: most products are putting **a chat panel** in front of everything. A chat panel is not a tiny core — it's a default. The discipline is to find the *surface-specific tiny core* that AI uniquely enables:

- **GitHub Copilot**: in-editor autocomplete in flow — that's a tiny core
- **Cursor**: agent edits over multiple files with diff approval — tiny core
- **Claude Code**: terminal-native agent with tool use — tiny core
- **Notion AI agent**: agent roaming the connected workspace (the workspace itself is the substrate, like Unix) — tiny core

For Copilot-style products that lack a clear tiny core, no amount of additional integrations will fix it.

---

## Related to Adjacent Concepts

- **[Naked Robotic Core](../concepts/naked-robotic-core.md)** — once you have multiple competing primitives, the work is consolidating back to the tiny core. Tiny Core is the principle; Naked Robotic Core is the consolidation discipline.
- **[Utility Curves](../concepts/utility-curves.md)** — Stewart Butterfield's S-curve view. The tiny core is what gets you *over the threshold* on the curve. Below threshold, no investment produces value; the tiny core is the unlock.
- **[We Don't Sell Saddles Here](../concepts/we-dont-sell-saddles-here.md)** — position the product by the transformation the tiny core enables, not by the surface feature.
- **You have to be right, not first** — Schoening's corollary. AirPods/MP3-player/Anthropic case study. Network effects exist but are overrated; the right tiny core wins late.

---

## PM Application

For a Senior Director of PM at Microsoft, in particular for Copilot:

1. **Apply the Tiny Core test to every Copilot surface.** Microsoft Copilot spans dozens of products: M365, GitHub, Windows, Edge, Bing, Sales, Service, Security, Studio. For each, ask: *what is the single elegant primitive that AI uniquely enables here?* If the honest answer is "a chat panel," that's not a tiny core. Force a better answer. (For M365: is it *cross-app context*? *Find-then-edit*? *Meeting-as-prompt*? Force the team to commit.)

2. **Use Tiny Core as the strongest possible no-vote on feature requests.** Standard PM defense ("we don't have bandwidth," "let's prioritize," "it's not a fit") all leave room for endless feature accumulation. Tiny Core gives you a sharper veto: *"This feature doesn't sharpen the core, it dilutes it. No."*

3. **Audit launched Copilot features by tiny-core fit.** Many existing Copilot features feel undifferentiated *because* they don't sharpen a tiny core — they're competent execution of generic AI assistant patterns. The Dropbox lesson: *push back to the core; resist surface expansion.* What is the in-flow primitive that the rest of the surface should defer to?

4. **For new surfaces: refuse to ship without a stated tiny core.** A new Copilot bet should be reviewable on one question: "What is the tiny core here, and how do we know users feel it?" If a product team can't articulate the tiny core in one sentence, the bet isn't ready.

5. **The 2014 Notion lesson is the warning.** It is possible to spend years polishing the wrong thing. The thing being polished can be objectively good — Schoening's editor was better than Notion's at the time. It still loses if the core isn't right. Microsoft has many polished surfaces. Polish is not a substitute for a tiny core.

---

## Sources

- [Lenny's Podcast — Max Schoening](../podcasts/lenny-max-schoening-agency-over-skills.md) — primary articulation with full catalog of examples, 2026-05-03

## Related

- [Naked Robotic Core](../concepts/naked-robotic-core.md)
- [Utility Curves](../concepts/utility-curves.md)
- [We Don't Sell Saddles Here](../concepts/we-dont-sell-saddles-here.md)
- [Malleable Software](../concepts/malleable-software.md)
