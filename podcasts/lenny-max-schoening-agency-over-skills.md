---
title: "Why Cultivating Agency Matters More Than Cultivating Skills in the AI Era — Max Schoening"
type: podcast
date_added: 2026-05-15
tags: [ai, product-strategy, leadership, career, org-design, frameworks, microsoft-relevant]
sources: ["https://www.lennysnewsletter.com/p/why-cultivating-agency-matters-more"]
related: ["../entities/max-schoening.md", "../entities/notion.md", "../entities/lenny-rachitsky.md", "../concepts/cultivating-agency.md", "../concepts/tiny-core.md", "../concepts/first-ten-percent-free.md", "../concepts/malleable-software.md", "../concepts/obviously-good.md", "../concepts/naked-robotic-core.md", "../concepts/small-group-theory.md", "../concepts/builder-vs-information-mover.md", "../concepts/dont-be-fungible.md", "../concepts/harness-as-moat.md", "../concepts/right-amount-agi-pilled.md"]
---

# Why Cultivating Agency Matters More Than Cultivating Skills in the AI Era

## Metadata

- **Show**: Lenny's Podcast: Product | Career | Growth
- **Guest**: [Max Schoening](../entities/max-schoening.md), Head of Product at [Notion](../entities/notion.md)
- **Host**: [Lenny Rachitsky](../entities/lenny-rachitsky.md)
- **Date Published**: 2026-05-03
- **Length**: 1:27:22
- **URL**: https://www.lennysnewsletter.com/p/why-cultivating-agency-matters-more

---

## Summary

Max Schoening — designer-engineer-PM hybrid (Google PM, Heroku design lead, GitHub design + engineering under Nat Friedman, two-time founder, now Head of Product at Notion) — argues that in the AI era, **agency**, not skills, is the rare and durable asset. As AI handles "the first 10% of every project" for free, the bottleneck shifts to people who will decide and ship. The episode also lays out his "tiny core" theory of great products, his long-held belief in **malleable software**, his skepticism of the SaaSpocalypse, and his contrarian read that intelligence has a "retina display" ceiling for most knowledge work.

---

## Key Takeaways

### 1. Agency > Skills

> "Before, it was very easy to always say, 'Well, I will never be able to do this because insert skill issue.' We're realizing that even if you have the skills at your fingertips, the thing that matters is agency. I don't think agency is very evenly distributed in the world."

The PM/designer who thrives is not the one with the strongest skill stack but the one who treats the world as malleable and acts on it. Schoening: "People who have true agency and understand that the world around them is malleable will do great. And the folks who stick to 'tell me really, what does it mean to be a PM? What does it mean to be a designer? And what's my job as an engineer?' — that will be much harder."

**How to cultivate it**: by **making things**, not by gaming an org chart. "When a lot of people hear agency, they think of themselves as in this big machine and they're going to circumvent their terrible boss. It's like, no, no, just start by making things. And usually when you get better at making things, at some point people pay attention, and it just really awakens you to the idea that you can just change things."

The deep source: a Steve Jobs riff. *"One day you wake up and you realize the world is made up by people no smarter than you."* Schoening: "There are basically people who realize this by themselves or they have an amazing teacher early on in their life that encourages this. And the biggest through line I've found is making."

See [Cultivating Agency](../concepts/cultivating-agency.md).

### 2. "Drive Notion Like It's Stolen"

Schoening's personal mantra and the operating norm he tries to install. The Notion design team is "above average agency compared to other places I've worked." Brian Levin is the canonical example — already blurs engineering and design, but *also* recruits aggressively because "this is what the org needs." Eric Lou asked: "If you started a startup, would you hire me in the first 10?" Schoening said no. Lou's response: *"Then I'm going to work on the skills so that you would hire me in the first five."* That led to him dropping PRDs for Figma, then dropping Figma for prototypes in code.

**The frame**: most employees behave like custodians of an existing role definition. High-agency people behave like founders even when they aren't — they reshape the role around the change they want to see.

### 3. The First 10% Is Now Free

> "The first 10% of every project are now free."

Project economics have inverted. The PRD, the initial prototype, the directional spike — these used to take days or weeks. Now they take an evening. Implication: *"Demos not memos"* (a GitHub-era principle Schoening brought to Notion). And: *"It's cheaper to just explore a lot of paths. You can now afford to say I'm going to send off 10 agents to explore 10 different things and then see if I was right."*

But the last 10% is still 90%. Easy first-90% does not produce shippable software; the hard work of polish, reliability, and "obviously good" remains.

See [First 10% Is Free](../concepts/first-ten-percent-free.md).

### 4. The "Tiny Core" Theory of Great Products

> "All the great products have something tiny that is a superpower, one tiny core that is so exceptionally good."

Schoening's catalog:
- **iPhone**: multitouch
- **GitHub**: the pull request ("anyone can suggest something to you and you see it")
- **Notion**: blocks + slash commands
- **Heroku**: `git push heroku master` — "that's so intoxicating that everything else flows from there"
- **Dropbox**: the menu bar icon — "it was better at figuring out whether you had an internet connection than your Mac itself"
- **Figma**: seamless blend between real-time collaboration and not
- **Snapchat**: disappearing photos

The trap: *"If I just add one more thing to the product, it'll be finally great. That never works."*

Schoening's failure-mode confession: in his 2014 Notion competitor, he polished editing (markdown folding, what's now in Obsidian) while Notion's first editor "was terrible — you couldn't even select between two blocks, but it turns out it didn't matter" because blocks were the tiny core.

See [Tiny Core](../concepts/tiny-core.md).

### 5. Stop Drawing Dead Fish (Bret Victor): Design AI in Code, Not Figma

Origin story for designers-shipping-code at Notion: the team was designing chat interfaces *in Figma*. Schoening, citing Bret Victor's "Stop Drawing Dead Fish": **the static image of a chat is the dead fish.** You can't feel AI in a mockup. Two designers + Schoening built an LLM-friendly playground (small, agent-friendly codebase, minimal-fear terminal experience) and moved chat prototyping there.

The point isn't shipping production code. *"I actually don't care at all whether designers write code that lands in production. The reason I like thinking in code is because it forces you to consider the medium."* The medium of AI products *is* agent loops. A designer who can tweak CSS but doesn't understand an agent loop is worse than one who deeply understands agent loops.

### 6. Malleable Software (a Schoening pre-AI belief now mainstream)

> "Software works closer to the interest of the people that use it than the interest of the corporation that makes it... Imagine you lived in an environment where you do not get to rearrange your living room and the kitchen has to be exactly set up the way that someone else decided. We would not take that. But that is kind of the world that we have in software right now."

Apps are too rigid — UI, data, behavior all glued together by the vendor. The opposite extreme (run your own Linux distro) is too costly. Malleable software splits the difference: communal tools that users can shape. Works with Geoffrey Litt (Ink & Switch) on this.

AI makes this suddenly accessible: people now make their own tools for their own workflows. *"It just has to be built on top of a platform or an operating system that encourages this, because otherwise we're just doing individual little tools. And I like communal tools."* Schoening sees Notion as that platform.

See [Malleable Software](../concepts/malleable-software.md).

### 7. SaaSpocalypse Skepticism

Pushback on "AI will gut SaaS." Schoening's argument:
- A lot of 2010s SaaS was a guided spreadsheet — and the guidance *is* the value.
- *"I've tried rebuilding Notion in a weekend for myself just to push at the edges of frustrating things. I don't think people want that. I think for the most part, it's nice if you can just go to Costco and have the steak in a styrofoam packaging and pretend that it wasn't hunting or an animal in the first place."*
- Software is a garden — you need to tend it (Bret Taylor). The "as a service" part is maintenance + specialists thinking hard about a problem.
- **Anthropic uses Slack**, despite being the AI lab most equipped to rebuild it. *"There's this graphic of what it takes to deliver a notification in Slack — that's just something that you only get to when you have real users, real scale, and decades of just 'yep, we understand the customer.'"*

Tools will become *more general* — back toward '90s general-purpose software (WordProcessor, spreadsheet, FileMaker Pro) — and stay as a service. Specialized tools survive on the edges where someone goes the extra mile.

### 8. Designers and PMs in the Terminal

Schoening actively prefers TUIs (Claude Code, Codex) over GUIs for designers and PMs. Reason: once in the terminal, *"they're going to be curious and pull at other threads. One day they wake up and they're like, oh, I understand more of the substrate of how computers work."* Terminal becomes the gateway drug to substrate understanding.

Designers at Notion now mostly code; some teams ask them to *reverse engineer* designs back to Figma so marketing can make videos — Schoening calls this "busy work" and a sign the medium has shifted.

### 9. Vibe Coding ≠ Quality Software

> "I don't feel like the quality of software has increased all that much in the last 12 months. I think maybe the amount of software has, but it's very, very hard to find software that is reliable."

The implicit critique of "vibe coding" success stories: the floor has not risen. Even the labs ship regressions every two weeks; their TUIs don't render at reasonable frame rates. Schoening wants the industry to recover *"Apple-esque, machined, unibody-aluminum"* engineering — a craft bar that AI-generated code has not produced.

See [Obviously Good](../concepts/obviously-good.md).

### 10. Software Is Still Eating the World — More, Not Less

> "I'm not that impressed with the progress in any other domain. It tends to be — I don't think they've gotten significantly better at writing. I still very much hate reading AI slop writing. But the thing is software. Andreessen — software is eating the world. Well, if the cost of software and creating software is going to zero, we will just have a lot more of it."

Models improve fastest at coding. Improvements in other domains are *coding principles applied to those domains*. The implication is that "AI eats jobs" is the wrong framing — software is eating jobs, and AI is the latest accelerant of that.

### 11. Intelligence Has a "Retina Display" Ceiling

For most knowledge work, model intelligence saturates. *"After I can't see the pixels, I can't see the pixels. I don't need you to make them smaller. Is it not the same for a lot of cognitive tasks?"*

The labs operate as if everyone always wants the frontier — true for cancer research, false for most knowledge work. *"Society is largely not capped by intelligence."* (Tyler Cowen cited as agreeing.) Past saturation, what matters is **speed of inference + modality**. If inference becomes instant, multitasking dies and direct manipulation returns — *"do you instantly mold the clay that is the code?"*

Connects to [Right Amount of AGI-Pilled](../concepts/right-amount-agi-pilled.md): once you accept saturation, you stop designing for "the next supermodel" and start designing for cheap, fast, possibly local models.

### 12. Token Spend Is a Bad Metric (But Leaderboards Have Their Place)

Notion's 1 PM is the highest token spender at the company. Schoening's policy: he doesn't track it. *"It's the wrong thing to optimize for. It's like when something new comes along, it's worth letting people explore."* In 6–12 months, *"a lot of companies are going to actually start asking questions around ROI, and I think that will be an uncomfortable conversation."*

Token-spend leaderboards are the new "lines of code." But: *"I have some sympathy for [Meta's leaderboard]. It is surprising to me how much prodding you need to do to get people out of the way they're used to working."* At Meta scale, public pressure is one of the few mechanisms that shifts default behavior.

### 13. Shots on Goal + "Obviously Good"

Two Notion-internal principles in tension:
- **Shots on goal**: increase experimentation rate.
- **Obviously good**: only ship things that are obviously good. *"I don't think anyone argued when they saw the first iPhone that it's obviously good. I don't think anyone argued that when ChatGPT first came out that it's obviously good. And so I think that's the bar."*

Resolved through **incremental correctness** — iterate aggressively toward obviously good, but iterate in public, not in a "cave in isolation."

See [Obviously Good](../concepts/obviously-good.md).

### 14. The "Naked Robotic Core" — Consolidation Discipline

Notion has *six automation primitives*. Claude desktop has three tabs (co-work / code / chat). Schoening: this is fine *during* exploration. But: *"You do have to do the hard work at consolidating it back into the naked robotic core of that idea... figure out what's actually the core simple thing that should outlive the other evolutionary branches of that same idea."*

The trap is shipping the next thing too fast and never consolidating. *"That's hard because you have to be okay with perhaps then shipping the next thing slightly delayed as you reconcile."*

See [Naked Robotic Core](../concepts/naked-robotic-core.md).

### 15. Taste = A Trained Model in Your Head

> "Taste actually means you're able to run a virtual machine in your head where, given an idea, you can predict for a certain in-group whether they're going to like it or not. You just have to do reps. It's almost like training a model."

Implications:
- You decide your in-group; you're not training for 8B people.
- Built by iteration + feedback (back-prop analogy). No shortcuts.
- High-taste designers at Notion are the ones with side projects *and* constant tool tinkering — high exposure rate to other people's ideas.
- Surround yourself with tasteful things. Notion conference rooms are named after objects (first typewriter, Macintosh, Porsche 911) so *"inevitably when I'm sitting in one of the rooms, nothing I'm doing amounts to this. I got to do better."*

Counterargument to the popular "AI takes everything; taste is what's left" frame: *"I'm not so sure — the loop is input idea, how do people react. That seems very back-prop. I don't know."* Taste is *also* trainable, including potentially in models.

### 16. Coding Agents as "the Operating Systems of the '90s"

Casual but load-bearing aside: *"All the coding harnesses are basically the operating systems of the '90s. And so I think that's why I care that people code, not because of the utility of shipping to production, but because it forces you to really interrogate the material that you're designing with."*

This is direct evidence for [Harness as Moat](../concepts/harness-as-moat.md) — the workspace harness is positioned as the substrate competition layer of this generation, not the model itself.

### 17. Make Users Superheroes (Kathy Sierra)

Why automated code review tools fail: *"You push your code, and a thing roasts your code and tells you how terrible of a developer you are. Versus Claude Code / Codex — you're coding and then you publish the work of you plus Claude and you get bragging rights of how good of a developer you are."*

Same product, opposite framing of the user. The superhero framing wins.

### 18. Notion's Agent Works Because Agents Need Context

Why Notion's AI agent landed well: *"Agents need context to operate in. Agents don't really like walls of 'I have to go through this narrow orifice to talk to this other data repository.' For the first time, it is obvious to people why a connected workspace is actually valuable, because... I can have agents roam around."*

A connected workspace is a **Unix-like environment for agents.** Schoening explicitly frames Notion as "an operating system." The decade of patient connected-workspace work suddenly became load-bearing for AI-era product market fit.

### 19. JTBD as an Antidote to "I'm an Employee Reviewing My Own Product"

Schoening's pragmatic take on Jobs-to-be-Done: not a sacred framework, but a useful prompt. *"In larger organizations, people turn off the brain when they're reviewing their own products. They're more like, 'I'm an employee of this company and I made a thing.' JTBD might encourage them to zoom out... be that user for a second. Would you even buy the thing that you just made?"*

### 20. Small Group Theory + Selective Inclusivity (Contrarian Corner)

> "I think the world is run by group chats of eight people or fewer. And so sometimes it's great to be exclusive."

Notion *could* aim for 8B users. If it did, it would alienate the top 500M, who want different things. *"Everybody is in the top of the class at something."* Caveat: this is about products, not labor markets — exclusive hiring practices in monopoly employment situations is not what he means.

See [Small Group Theory](../concepts/small-group-theory.md).

### 21. "We Already Have Universal Basic Income — It's Called Knowledge Work"

Half-joke, half-real. *"If you really look at what we actually need to live and to be content, it is a lot less. And we've built this hierarchy and all these jobs... So we already have UBI. We'll come up with other ways in which we as humans, because we're the most important species in the universe, insert ourselves into the conversation around agents."*

The deep claim: humans will keep inventing reasons they must be in the loop. Frenetic AI-era career anxiety is misplaced.

### 22. Don't Take "The Last Train Out"

Closing counsel to younger people in Silicon Valley: *"Silicon Valley is uncharacteristically full of people who don't actually love computers... There's this idea that this is the last train, the permanent underclass. It is so detrimental to thinking about how you want to spend your heartbeats."*

The advice: work very hard from 18 to 25, then less. But don't let frenzy distract from what you actually care about. Read history. Read computer science history.

---

## Notable Quotes

- "Cultivating agency matters more than cultivating skills."
- "Do you drive Notion like it's stolen?"
- "The first 10% of every project are now free."
- "Demos not memos."
- "Every time there is a human intervention [in code], it should feel a little bit like a bug." (Schoening citing Simon Willison)
- "The last 10% are still actually 90%."
- "All the great products have something tiny that is a superpower."
- "You have to be right, not first."
- "Just make obviously good stuff."
- "Software is a garden — you need to tend to it." (Bret Taylor)
- "All the coding harnesses are basically the operating systems of the '90s."
- "Taste actually means you're able to run a virtual machine in your head."
- "We already have universal basic income. It's called knowledge work."
- "The world is run by group chats of eight people or fewer."
- "One day you wake up and you realize the world is made up by people no smarter than you." (Steve Jobs, via Schoening)
- "You can just change things."

---

## Frameworks Introduced

- **[Cultivating Agency](../concepts/cultivating-agency.md)** — agency is the durable AI-era asset; cultivated by *making*, not by gaming the org
- **[Tiny Core](../concepts/tiny-core.md)** — great products win through one exceptional core mechanic, not feature breadth
- **[First 10% Is Free](../concepts/first-ten-percent-free.md)** — AI inverts project economics; the last 10% is still 90%
- **[Malleable Software](../concepts/malleable-software.md)** — software should serve user interest, not vendor interest
- **[Obviously Good](../concepts/obviously-good.md)** — only ship things that are unmistakably good; iterate to get there
- **[Naked Robotic Core](../concepts/naked-robotic-core.md)** — consolidation discipline after divergent exploration
- **[Small Group Theory](../concepts/small-group-theory.md)** — the world is run by 8-person group chats; be okay with exclusive

## Frameworks Referenced (not introduced)

- **Stop Drawing Dead Fish** (Bret Victor) — invoked to justify prototyping AI in code
- **[Jobs to Be Done](../books/christensen-competing-against-luck.md)** (Christensen) — pragmatically; antidote to org-blindness
- **Make users superheroes** (Kathy Sierra) — code review tools framing
- **Software is eating the world** (Marc Andreessen) — accelerating, not slowing
- **The timeless way of building** (Christopher Alexander), **How Buildings Learn** (Stewart Brand) — malleable software's physical analogs
- **Software is a garden** (Bret Taylor)
- **Manual intervention is a bug** (Simon Willison) — in the code-writing loop

---

## PM Relevance

For a Senior Director of PM at Microsoft, the most actionable claims:

1. **Make agency a hiring rubric — not a slogan.** Existing rubrics emphasize impact, scope, and influence — all of which a high-skill, low-agency PM can score on by working through hierarchy. Add an explicit agency signal: *"Show me something you shipped without being asked. What did you have to push past to ship it?"* If the answer is a workflow shortcut, an internal tool, a side-project prototype, that's agency. If it's "I aligned stakeholders to ship X," that's information movement. Connect this to [Builder vs. Information Mover](../concepts/builder-vs-information-mover.md).

2. **Audit whether your org actually rewards "drive it like it's stolen."** Large companies systematically punish high-agency behavior through process gates, alignment rituals, and the requirement to socialize before deciding. If a Notion-style "ship the prototype before the PRD" move would get a Microsoft PM in trouble, the rhetoric is hollow. Specific fix: identify and *publicly reward* one Eric-Lou-style story per quarter — someone who reshaped their role by making.

3. **Push PMs and designers into the terminal — literally.** Claude Code / Codex over Figma for AI surfaces. Not because they should ship production code, but because *the medium of AI products is the agent loop*, and the agent loop only lives in code. A Copilot PM who can't reason about an agent loop is designing for a phantom of the actual product. Fund tooling, training, and the org permission to spend time here.

4. **Apply the Tiny Core test to every Copilot surface.** Microsoft's AI strategy spans dozens of products (M365 Copilot, Copilot for Sales, Copilot Studio, GitHub Copilot, Windows Copilot, Edge Copilot, Bing). For each: *what is the single elegant primitive AI uniquely enables here?* If the honest answer is "a chat panel," that's not a tiny core — that's a default. The discipline is to find the surface-specific primitive (e.g., for GitHub Copilot it's arguably *autocomplete in flow*; for M365 Copilot is it *cross-app context*? *Find-then-edit*? *Meeting-as-prompt*?). Force the answer; refuse the chat panel.

5. **"First 10% is free" reshapes performance reviews.** "I built a prototype" is the new baseline, not differentiated work. The promo case question shifts to: *what happened in the middle 80%* — the slog from demo to shippable, the consolidation, the obviously-good polish. Calibrate review rubrics accordingly.

6. **Don't bet against SaaS internally.** M365, GitHub, Azure are not in structural decline because of AI — they're in structural expansion if executed. The strategic narrative inside the building should reflect this. The risk Schoening flags is *complacency*, not displacement.

7. **Use the "obviously good" bar against feature creep.** When a Copilot review presents "feature N+1," the question isn't "is this good?" — it's "would anyone say *obviously good* about this?" If not, kill it or fix it. Pair with shots-on-goal: more concurrent bets, fewer mediocre ships.

8. **The Naked Robotic Core principle applies to Copilot surfaces too.** Microsoft has many Copilot brands and entry points — chat panel, side panel, in-line, full app, agent builder. At some point the consolidation work has to happen: what is the *one* primitive Copilot is, and what are the evolutionary branches that should be pruned? Schoening would say this work is uncomfortable but mandatory.

9. **Treat connected workspace as a Microsoft superpower the same way Notion does.** Schoening's read on why Notion's agent landed: connected workspace = Unix for agents. **Microsoft Graph + M365 is a vastly larger version of the same asset.** The strategic move isn't "build a better model"; it's "make Graph the substrate agents naturally run on." This is [Harness as Moat](../concepts/harness-as-moat.md) at enterprise scale.

10. **Intelligence-retina-display is a hedging hypothesis for Microsoft.** If Schoening (and Cowen) are right that most knowledge work hits an intelligence ceiling, then the right portfolio bet is: don't depend exclusively on always running the frontier model. Invest in fast, cheap, local, multimodal — and in the workspace harness that absorbs them.

---

## Entities

- [Max Schoening](../entities/max-schoening.md) — guest
- [Lenny Rachitsky](../entities/lenny-rachitsky.md) — host
- [Notion](../entities/notion.md) — Schoening's current employer
- People referenced: Ivan Zhao (Notion founder), Simon Last (Notion eng), Brian Levin/Lovin (Notion designer — high-agency example), Eric Lou (Notion PM example), Nat Friedman (GitHub), Bret Victor, Bret Taylor, Geoffrey Litt (Ink & Switch), Steve Jobs, Brian Chesky, Dieter Rams, Frank Gehry, Stewart Brand, Christopher Alexander, Clayton Christensen, Kathy Sierra, Cat Wu, Marc Andreessen, Simon Willison, Tyler Cowen, Dario Amodei, Mitchell Hashimoto, Lee Sedol, Marcus Aurelius

## Concepts

- [Cultivating Agency](../concepts/cultivating-agency.md) — the central thesis
- [Tiny Core](../concepts/tiny-core.md)
- [First 10% Is Free](../concepts/first-ten-percent-free.md)
- [Malleable Software](../concepts/malleable-software.md)
- [Obviously Good](../concepts/obviously-good.md)
- [Naked Robotic Core](../concepts/naked-robotic-core.md)
- [Small Group Theory](../concepts/small-group-theory.md)
- [Builder vs. Information Mover](../concepts/builder-vs-information-mover.md) — agency is the underlying disposition that distinguishes builders
- [Don't Be Fungible](../concepts/dont-be-fungible.md) — agency complements the non-fungible-combination thesis
- [Harness as Moat](../concepts/harness-as-moat.md) — "coding harnesses are the operating systems of the '90s" is direct evidence
- [Right Amount of AGI-Pilled](../concepts/right-amount-agi-pilled.md) — intelligence-retina-display is a related claim

## Books Mentioned

- [Code: The Secret Language of Hardware and Software](../books/petzold-code.md) by Charles Petzold
- [Tools of Conviviality](../books/illich-tools-of-conviviality.md) by Ivan Illich
	- [Seeing Like a State](../books/scott-seeing-like-a-state.md) by James C. Scott
- *Project Hail Mary* by Andy Weir (lightning round; not added)
- *The Timeless Way of Building* (Christopher Alexander), *How Buildings Learn* (Stewart Brand) — referenced for malleable software

## Other Products Mentioned

- Ghostty (Mitchell Hashimoto's terminal emulator)
- Corne (split keyboard, open-source)
- Moshi (phone product)
- CIVIVI (pocket knife)
- Vercel (compared to Heroku)
- Cluely (cited as anti-pattern for durability)
