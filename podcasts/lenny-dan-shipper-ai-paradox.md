---
title: "The AI Paradox: More Automation, More Humans, More Work — Dan Shipper"
type: podcast
date_added: 2026-05-27
tags:
  - ai
  - product-strategy
  - saas
  - org-design
  - agentic-ai
  - frameworks
  - microsoft-relevant
sources:
  - https://www.lennysnewsletter.com/p/the-ai-paradox-dan-shipper?showTranscript=true
related:
  - ../entities/dan-shipper.md
  - ../entities/every.md
  - ../entities/lenny-rachitsky.md
  - ../concepts/automation-is-a-lie.md
  - ../concepts/forward-deployed-engineer.md
  - ../concepts/bring-your-own-tokens.md
  - ../concepts/super-agent.md
  - ../concepts/ride-the-model.md
  - ../concepts/reach-test.md
  - ../concepts/harness-as-moat.md
  - ../concepts/builder-vs-information-mover.md
  - ../concepts/malleable-software.md
---

## Metadata

- **Show**: Lenny's Podcast
- **Episode**: The AI Paradox: More Automation, More Humans, More Work
- **Guest**: Dan Shipper — co-founder & CEO of [Every](../entities/every.md)
- **Host**: [Lenny Rachitsky](../entities/lenny-rachitsky.md)
- **Date Published**: 2026-05-24
- **URL**: https://www.lennysnewsletter.com/p/the-ai-paradox-dan-shipper

---

## Summary

Dan Shipper makes three buckets of falsifiable predictions for May 2027 (Lenny will score them in a year): (1) **how work happens** — bifurcates into a company-wide super-agent in Slack plus all-other-work-happens-inside-Codex-or-Cowork; (2) **the shape of work** — non-technical staff ship PRs, technical staff garden agent ecosystems, AI-written docs get normalized; (3) **who thrives** — PMs and full-stack designers ("PM Designer thriving"), forward-deployed engineers, and anyone who rides each new model. The unifying thesis is the **AI paradox**: automation creates more humans and more work, because *"every agent needs a human who cares about it."* He also makes one specifically contrarian financial call — *"I would buy SaaS stocks right now. I think the SaaSpocalypse is dumb."*

---

## Key Takeaways

### 1. "Automation is a lie" — the AI paradox

> "Automation is a lie, in the sense that every time you automate something, in order to make sure the automation is working well you need a human on top of it making sure that it's working well."

> "I'm simultaneously extremely AI-pilled, extremely, and very bullish on humans and the role of humans and making sure that AI is working well."

The mechanism, in Shipper's exact framing:

> "What models do in general is they make yesterday's human competence cheap. And so it becomes commoditized. It's not valuable anymore. What humans do is we go in there and we're like, 'Yeah, we have all this frozen human competence from yesterday. How do I use this to make something new and interesting?'"

Empirical anchor: Every doubled headcount in the last year (15 → ~30) while running six internal AI products. Shipper: *"We have so much automation, so much AI, and I also work way more."* (See [Automation Is a Lie](../concepts/automation-is-a-lie.md).)

### 2. Work bifurcates: one super-agent in Slack + everything else in Codex/Cowork

Shipper flipped his earlier prediction. He used to think personal agents would win — "a little daemon on your shoulder" like Pullman's Golden Compass — and was very into OpenClaw. He has now *"completely flipped"*:

> "And then everyone realizes it's like way too much work. This thing breaks all the time. I got to fumble around with it. I got to be able to SSH into my server and like blah, blah, blah... the fundamental, underlying thing that drives that is whether it's OpenClaw or any other harness, in order for an AI agent to be useful right now, it really needs a human who cares about it."

The architecture that's emerging: one canonical company-wide super-agent (Shopify's "River," Ramp's similar one, Anthropic/OpenAI internally) plus team-level specialization that trickles down as models get better. (See [Super-Agent](../concepts/super-agent.md).)

Brandon Gell, Every's COO, coined the work/personal split: *"There's this whole territory of using personal agents for your computer errands. It's like order my groceries or whatever."* Work agents in Slack; computer errands stay personal.

### 3. Codex/Cowork is the new workspace — and SaaS runs inside it

> "Most of the work that you do is actually going to happen on your computer, in an environment like Codex or Claude Cowork. That becomes the operating system for ... it becomes an operating system for how you do all of your work, whether that's your email, the documents you create, all that stuff."

The architectural insight is that Codex put a **browser inside the agent**, not the agent inside the browser:

> "For a long time, I thought too that the optimal experience of AI was going to be take AI and put it in a browser. And I think the reverse is actually starting to happen and be really, really valuable in a way that I did not expect, which is take the AI agent that you use all the time on your computer and put a browser in it so it can see everything you're doing."

His daily-driver workflow: one Codex thread per project, in-app browser open to Proof (Every's open-source markdown editor), Codex watching what he's doing and acting in parallel. *"I've been at inbox zero for 10 days straight now, which if you know me, is crazy"* — Quora (Every's email agent) gathers emails, renders a page, and he monologues at it.

### 4. CLIs are over — *"we speed ran the CLI era"*

> "CLIs are over. We speed ran the CLI era. It was nice while it lasted... when you move into an actual UI for this, you start to realize we made GUIs for a reason, and it's just nicer to be in a GUI, and you can get all the same benefits inside of a GUI, especially for non-programmer work."

Important caveat — CLIs *won't disappear* (they've been around 40+ years); they just stop being the dominant agent surface. Most technical staff at Every have already moved off CLI as their main work surface to Codex/Claude Code/Cursor.

### 5. SaaS thrives because users bring their own tokens

> "I would buy SaaS stocks right now. I think the SaaS apocalypse is dumb, and SaaS stocks will be up majorly in the next couple years."

The mechanism, with Every's own Proof as the worked example:

> "When I run the agent on that website, I'm using my tokens. I'm not using the vendor's tokens, I'm not using the app's tokens... For example, with Proof, for anyone who uses it, I don't pay for tokens because they bring their AI to Proof. And so it changes what you build as a SaaS company and you build it now for both humans and agents to use at the same time, and it changes your margins back to, well, I don't really have to pay for tokens anymore because the user's going to bring AI."

> "What agents do is increase the number of users of SaaS, not get rid of it. And so I think SaaS companies are going to see an insane spike in the amount of demand that they have, because there's going to be tons of agents using these products at a very high volume."

Every's own SaaS spend is *up* year-over-year despite being maximally AI-forward. (See [Bring Your Own Tokens](../concepts/bring-your-own-tokens.md).)

### 6. Forward-deployed engineer is the most essential new hire

> "The whole forward-deployed engineer concept I think is for real and it comes out of every agent needs a human. You go to the big model companies, they have these agents that run internally, they have teams of people that run these agents and I don't think those teams are going away."

Named example: **Nitesh** at Every — *"an AI engineer and he fits this sort of forward deployed category... He spends most of his time actually talking to one of our agents in Slack. We have an agent internally called Claudy, which runs our whole consulting practice and he spends a lot of time in Slack."*

Framing tweak Shipper insists on:

> "I would sort of split it into less babysitting agents and more your forward deployed team is trying to build a whole system that makes it so that people who have less knowledge can use that system without doing something dumb. And that's like a really interesting engineering challenge."

Anti-pattern to avoid: data scientists hating their lives because they're reviewing bad agent-produced analyses. Solution at one big lab: a dedicated data science bot, *"that every single person in the org can query that is hooked up to their data warehouse that knows who's who so that it knows at the warehouse level who has permission to access what."* The FDE team builds the bot; the data scientists go deeper on harder questions. (See [Forward-Deployed Engineer](../concepts/forward-deployed-engineer.md).)

### 7. PMs thrive — Marcus on Spiral is the evidence

> "I am super, super bullish on PMs."

The example: **Marcus** runs Spiral (Every's writing app). PM by training; previously ran Axios' writing product. *"He took a year off that job and just got super AI-pilled and just learned how to use cursor basically really well... I would call him lightly technical, like knows what a database migration is."*

> "We never could have hired him to do this job even a year ago, but the coding models have gotten good enough that he can pair the technical knowledge that he does have with his really spiky product sense and sense for writing and sense for users and it's so dangerous. He ships faster than almost anyone on the team."

This is independent corroboration of [Builder vs. Information Mover](../concepts/builder-vs-information-mover.md) — builder PMs win; lightly technical + spiky judgment beats both pure technical and pure synthesis.

### 8. Full-stack designers become "superheroes"

> "If you're a designer and you're in these tools all the time, you're so used to, okay, I make this beautiful interaction and the engineer just doesn't want to do it... I see so many designers for us internally or externally where they now feel so empowered to go build stuff because they're like, 'I have all these ideas to make things look amazing and these interesting interactions.' And that's the exact thing that it's really hard to do with vibe coding because it just all looks the same. So it all looks like slop and they can make stuff that looks so different and now they can actually build it... a lot of times they just make pull requests."

Lenny's leading-indicator data point: designer roles on the job market have *not* grown. If they start to, that's the signal.

### 9. AI-generated writing gets normalized

> "We will be reading way more AI generated writing in documents and emails and we will like it."

Empirical: at Every's end-of-2025 quarterly planning, every team member talked to a Notion Agent that asked them about prior year, goals, metrics, pushed back, then synthesized into a strategy report. *"I got these incredibly good AI generated strategy reports or quarterly plans for each part of each team. And then I could go in and be like, 'Okay, who needs to talk to each other?'"*

The social rule Shipper proposes:

> "My expectation is if you send me an AI generated document, I think that's great. And if we talk about it and it's clear you have no idea what's in it, big no-no, not allowed to do that."

> "The kind of strategy document that GPT 5.5 can write when it's directed well by someone on my team is way better than them just like dinking and dunking their fingers on the keyboard."

### 10. Ride the model — the survival strategy

> "The only thing you need to do is ride the models and that means use them for whatever it is that you do."

Mechanism: each new model release re-opens previously-impossible problems. *"There are certain things where I know it can't quite do it yet, but when a new model comes out, I always turn the rock over again to be like, 'Can I do it now?'"* (See [Ride the Model](../concepts/ride-the-model.md).)

> "The edge of AI is wherever AI meets a real human doing something because the people at San Francisco, they're making it, but they don't actually know a lot about how to use it... whenever a new model comes out, you get to be one of the first people in the world to discover what it might be useful for."

Shipper's adoption diagnostic — the "reach test":

> "One of the things that we talk about internally is what I call the reach test, which is like, when you wake up in the morning, do you reach for it organically?"

(See [Reach Test](../concepts/reach-test.md).)

---

## Notable Quotes & Arguments

### The senior engineer benchmark (Shipper's own)

Shipper vibe-coded Proof on the side, it kept crashing in production, two senior engineers independently rewrote it, those rewrites became his benchmark.

> "All the models until GPT 5.5 got like a 30 out of 100, and a human senior engineer gets like high 80s, low 90s out of 100. So, there's a lot to go. And then I tried GPT 5.5 and it got like a 62. And mind you, the 60 score was GPT 5.5 using an Opus 4.7 plan. Opus 4.7 plans are very good; GPT 5.5 is the only model though that has the sense of agency and confidence to just like rip out old code and just actually rewrite from first principles. Other coding models, they end up papering over the edges."

The deeper point: benchmarks measure problems we've already framed, scored, and can articulate. The real human work of *deciding the frame* is invisible to benchmarks. *"Even if the benchmarks get saturated, it doesn't mean the same thing as you totally replace all senior engineers."*

### "Pete gets thousands of pull requests a day on OpenClaw and then he just spins up 50,000 Codex instances and then sorts through them and then merges a thousand of them."

The new shape of work: parallelism on the agent side; judgment-loaded triage on the human side. *"It brings up a lot of really interesting questions around which pull requests should you merge."*

### GitHub at agent scale

> "This is exactly why GitHub is having problems right now because the number of people using GitHub is skyrocketing exponentially and it's really just people's agents in GitHub."

### Agent bug reports

> "When someone has a problem they don't email support. Their agent sends a bug report, and an agent bug report is way better than a human bug report. It has 'here's exactly what I did, here's the exact repro steps, here's what I think is going on in the code base.' And then we just get that, it becomes a GitHub issue, and then we can just send off an agent to fix it."

### Two agents are better than one

> "When I have Codex interact with another agent, it can give so much more context about me and what I want than I would be able to type, and it can go back and forth talking about things that would take a long time for me to express directly to an agent."

Concrete instantiation: hosted OpenClaw onboarding — they *paused* the product (too hard to maintain) — but the architectural lesson stuck. Instead of building an onboarding flow, just require users to come via Codex/Cowork. Codex already knows everything about the user; it just talks to the app.

### CEOs are the laggards

> "CEOs and investors, it seems still very, very optional whether or not they use this stuff. I think the opposite is actually true. My experience... is that your company's only going to go as far as your CEO goes in AI and it's not something you can delegate. You have to have your hands in it because otherwise you don't have an intuition for it."

### The middle-ages-horizon framing

> "I think generally our intuitions about the future, the model that I have of what our intuitions are about the future is the intuitions that people had in the Middle Ages about what happened at the end of the horizon. It's like, are there dragons? Does it drop off into nothingness... And what happens is you get there and you're like, there's some really cool things, there's some not cool things and it's just another horizon."

---

## Frameworks Introduced

- **[Automation Is a Lie](../concepts/automation-is-a-lie.md)** — the headline thesis: every agent needs a human who cares about it; oversight work expands as automation scales.

- **[Super-Agent](../concepts/super-agent.md)** — one canonical company agent in Slack (Shopify "River," Ramp, Anthropic, OpenAI). Shipper's flip from personal agents.

- **[Bring Your Own Tokens](../concepts/bring-your-own-tokens.md)** — user-supplied inference budget improves SaaS margins; Proof is the worked example.

- **[Forward-Deployed Engineer](../concepts/forward-deployed-engineer.md)** — most essential new hire; named example Nitesh at Every running Claudy.

- **[Ride the Model](../concepts/ride-the-model.md)** — survival principle. "Models make yesterday's human competence cheap." Try every new release; turn over rocks; the edge of AI is wherever AI meets a real human doing something.

- **[Reach Test](../concepts/reach-test.md)** — Shipper's adoption diagnostic. Do you reach for it when you wake up?

- **Allocation economy** (Shipper essay reference) — humans work with AI by managing it, like a manager; *"managers actually spend a lot of time working."*

- **"Computer errands"** (Brandon Gell, Every COO) — the personal-agent territory distinct from work agents; grocery ordering, scheduling.

- **Three-bucket prediction structure** — Lenny's interview architecture, useful for future "year-out predictions" pieces.

---

## PM Relevance — Specific to Microsoft

1. **Re-frame Copilot's pitch from time-saved to amplification.** Shipper's "automation is a lie" arrives the same week as Microsoft's quarterly Copilot ROI narrative. The empirical truth is amplification, not replacement. Re-tool ROI calculators, sales decks, and customer success metrics around *output per knowledge worker* and *things attempted that wouldn't have been attempted before*, not *hours saved.* The savings story doesn't survive customer renewal conversations; the amplification story does. Pair with [Builder vs. Information Mover](../concepts/builder-vs-information-mover.md).

2. **Teams as the super-agent surface — and the strategic urgency of doing it before fragmentation hardens.** Shipper's flip is decisive: companies converge on *one* canonical agent in their primary chat tool, not many. Shopify shipped River. Ramp shipped theirs. Anthropic and OpenAI both run internal super-agents. The Microsoft question: is Teams positioned and shipped as the cross-functional super-agent for enterprise, or as a per-app sidekick that loses to a competitor's super-agent? If Slack ships a better super-agent surface before Teams does, the M365 install base will not save the seat.

3. **GitHub Copilot's competitive surface is now Codex / Cowork, not VS Code completion.** Shipper says Codex is his daily driver and "in the lead right now" — *"It's funny. People are like, 'Oh, are you sponsored by OpenAI?' I'm like, 'No, I just talk about what I like.'"* He's the most credible third-party voice in agent tooling. GitHub Copilot's strategic question shifts from "best in-editor experience" to *"are we the workspace where the knowledge worker spends the day?"* If the answer is no in 12 months, the rest of GitHub doesn't fix it. See [Harness as Moat](../concepts/harness-as-moat.md).

4. **GitHub's scaling pain is a feature, not a bug — but it's an early warning.** Shipper says GitHub is being crushed by agent traffic. That is *demand validation* for the agent-native workspace thesis, and it's also a leading indicator that the infrastructure layer is going to determine winners. Build for agent-rate-traffic in every product surface, not human-rate-traffic.

5. **Hire and visibly promote a "forward-deployed engineer" job ladder.** Microsoft's FDE-equivalent work is split across MCS, Industry Solutions, GSI partners, and field engineering. Shipper's prediction is that this role becomes a strategic asset, not a services cost line. The action: create a named, leveled, equity-participating FDE role inside product engineering — not consulting — whose explicit job is shipping product-aware agent customizations inside top enterprise accounts and feeding the customization surface (Copilot Studio, Power Platform, Graph extensibility) with what they learn. Anthropic and Palantir already run this way.

6. **BYOT is a Microsoft-positive arbitrage if internal incentives don't block it.** Microsoft sells both the substrate (M365 Copilot) and the inference (Azure OpenAI, Anthropic-on-Azure). The right move on Shipper's prediction is to enable BYOT on M365 Copilot for enterprise — and *also* offer preferred Azure inference for customers who bring their tokens. The risk is M365 economic models that disincentivize BYOT because it cannibalizes seat-attached inference margin. The correct lens: customer chooses; capture them on whichever rail. See [Bring Your Own Tokens](../concepts/bring-your-own-tokens.md).

7. **Designer roles are a leading indicator.** Lenny's market-data observation — designer hiring has not grown — paired with Shipper's "full-stack designers become superheroes" claim creates a clean check. Watch designer hiring in 12 months. If it spikes, the hybrid-design discipline is real. Microsoft should be hiring against the spike *now*, not after.

8. **"Ride the model" is the cultural norm to push internally.** Shipper's specific complaint: *"a lot of companies handicap their employees from even doing this because I don't know if you can use the latest models at Salesforce."* Microsoft has historically taken months to internally roll out frontier external models. The "ride the model" norm requires the opposite: internal access to the frontier on day one. The intuition Shipper is naming is correct — the people who *play* with new models the hour they drop find product capabilities their PMs and execs will not. See [Ride the Model](../concepts/ride-the-model.md).

9. **The "reach test" is the right Copilot North Star.** Not DAU, not MAU, not "asked-a-prompt" — does the user *reach* for Copilot when they sit down at the desk in the morning? Instrument it. The reach test eliminates a lot of vanity engagement metrics in a Copilot-instrumentation review. See [Reach Test](../concepts/reach-test.md).

10. **The "AI-written docs are fine if you stand behind every line" social rule should be policy at Microsoft.** Shipper's rule cuts the AI-document anxiety cleanly. Internally, Microsoft can adopt it: AI-written docs are welcome; the author must stand behind every line. This sets a productive culture norm without falling into either AI-document maximalism or AI-document panic.

11. **Watch for "work-like activity" expansion under agents.** Shipper warns that triaging 50,000 agent PRs to merge 1,000 is the new shape of work. If Microsoft's agent products produce *volume-loaded* oversight (review N agent diffs) rather than *judgment-loaded* oversight (decide what the agent should attempt), they degrade into [Hyper-Realistic Work-Like Activities](../concepts/hyper-realistic-work-like-activities.md). The right design target: agent surfaces where the human's role is choosing direction, not stamping artifacts.

---

## Lightning Round

- **Books recommended**: Annie Dillard, *The Writing Life* (required reading at Every — last chapter especially); Winston Churchill, *The Second World War* (combination history + memoir; Shipper sees parallels to Every's "build and write" stance); *The Rigor of Angels* (Heisenberg / Borges / Kant — AI-relevant philosophy of ideas).
- **Recent show**: *The Dark Wizard* (Dean Potter free-solo / wingsuit doc); also *100 Foot Wave* (big-wave surfing).
- **Product recently discovered**: Codex.
- **Life motto**: *"Do things worth writing about and write things worth reading"* (Shipper's college-era line). Plus Rob Burbea's *"relate to it from a position of spaciousness and strength"* — used personally when sitting with AI-career fear.
- **Underrated AI tool**: Codex again (told Boris Cherny and Cat Wu directly at the Anthropic Code with Claude event).
- **Mythos preview** (Anthropic): METR benchmark — can do 17-hour autonomous tasks at 50% accuracy.

---

## Entities

- [Dan Shipper](../entities/dan-shipper.md) — co-founder & CEO of Every
- [Every](../entities/every.md) — 30-person AI-native media + tools company; running lab
- [Lenny Rachitsky](../entities/lenny-rachitsky.md) — host
- Named at Every: **Marcus** (PM, runs Spiral writing app); **Nitesh** (AI engineer / forward-deployed; runs Claudy agent for consulting); **Brandon Gell** (COO, coined "computer errands"); **Pete** (OpenClaw maintainer, thousands of PRs/day)
- External references: **Shopify "River"** super-agent; **Ramp** super-agent; **Anthropic** internal agent teams; **OpenAI** internal data-science bot; **Cursor** (~recently acquired-adjacent by SpaceX, per Shipper); **Devin** (early autonomous-coding bet); **Hermes** (agent product Shipper recommends for technical users); **Victor**, **OnePlus** (less-technical agent options); Geoffrey Litt / Ink & Switch (malleable software, indirectly via "agents in apps")
- Books: Annie Dillard, *The Writing Life*; Churchill, *The Second World War*; *The Rigor of Angels*

---

## Concepts

- [Automation Is a Lie](../concepts/automation-is-a-lie.md)
- [Super-Agent](../concepts/super-agent.md)
- [Bring Your Own Tokens](../concepts/bring-your-own-tokens.md)
- [Forward-Deployed Engineer](../concepts/forward-deployed-engineer.md)
- [Ride the Model](../concepts/ride-the-model.md)
- [Reach Test](../concepts/reach-test.md)
- [Harness as Moat](../concepts/harness-as-moat.md) — Codex/Cowork as the new workspace
- [Builder vs. Information Mover](../concepts/builder-vs-information-mover.md) — Marcus / Spiral is the new exemplar
- [Malleable Software](../concepts/malleable-software.md) — adjacent: "humans and agents are on the same piece of work together"
- [Hyper-Realistic Work-Like Activities](../concepts/hyper-realistic-work-like-activities.md) — risk that agent oversight degenerates into the same trap
