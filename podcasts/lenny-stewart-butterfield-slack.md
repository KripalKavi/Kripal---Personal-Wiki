---
title: "Slack Founder: Mental Models for Building Products People Love"
type: podcast
date_added: 2026-04-19
tags: [product-strategy, frameworks, leadership, design, startups, microsoft-relevant]
sources: ["https://www.lennysnewsletter.com/p/slack-founder-stewart-butterfield"]
related: ["../entities/stewart-butterfield.md", "../concepts/we-dont-sell-saddles-here.md", "../concepts/utility-curves.md", "../concepts/hyper-realistic-work-like-activities.md"]
---

# Slack Founder: Mental Models for Building Products People Love

**Show**: Lenny's Podcast
**Guest**: [Stewart Butterfield](../entities/stewart-butterfield.md), co-founder of Slack and Flickr
**Host**: Lenny Rachitsky
**Published**: 2025-11-20
**Source**: https://www.lennysnewsletter.com/p/slack-founder-stewart-butterfield

---

## Summary

Stewart Butterfield — co-founder of Flickr and Slack, sold to Salesforce for $27.7B — shares the mental models behind both companies. The episode is unusually framework-dense: utility curves, Owner's Delusion, Hyper-Realistic Work-Like Activities, comprehension vs. friction, Parkinson's Law, and the full backstory on "We Don't Sell Saddles Here." Butterfield rarely does podcasts; this is one of the most substantive product strategy conversations he's given.

---

## Key Takeaways

### Utility Curves — The S-Curve of Product Value

See [Utility Curves](../concepts/utility-curves.md) for the full framework. The short version:

- Features aren't binary (have it / don't have it) — they exist on an S-curve of value delivery
- At the beginning of the curve: effort put in doesn't create much value yet (below threshold)
- In the steep middle: a small amount of additional investment creates enormous value
- At the end: continued investment yields diminishing returns — you've "done" this feature
- The question for every feature: are we on the first flat part, the steep part, or past the cliff?

Compounding factor: **divine discontent** (Bezos' term). The quality bar moves continuously. Users' expectations rise as software improves. A feature that was "good enough" two years ago may now be below the threshold of usefulness — and it won't get improved because it was shipped once and considered done.

Google Calendar's time zone picker: used by hundreds of millions of people, shows all time zones alphabetically by country, unchanged for years. If you're in California and want to set a meeting for New York time, your first result for "East" is "Eastern Australia, New South Wales." The utility bar has moved; the feature hasn't. This is the category of thing that erodes emotional connection over time.

---

### Comprehension vs. Friction — The More Important Distinction

The product mantra "reduce friction" is wrong in most cases. The actual challenge is usually **comprehension**:

**High-intent scenarios** (reduce friction): Ticketmaster for Taylor Swift tickets. The user knows exactly what they want, specificity and intent are maxed. Reduce clicks, speed up checkout — it matters here.

**Low-intent scenarios** (comprehension problem): Someone visits Slack.com. They've heard about it vaguely. Intent is barely above zero. Specificity is near zero ("it's a work thing... like a spreadsheet or calendar?"). Getting them to the signup form faster doesn't help if they have no idea what they're signing up for.

Butterfield's estimate: **70–80% of product design work lives in the comprehension problem**. People don't take advantage of most features because they never understood what those features do. Not because the path to the feature was too long — because they didn't know the feature existed or couldn't predict what it would do.

Two forms of comprehension failure:
1. "What is this thing?" — users can't understand what the product/feature does
2. "What am I supposed to do next?" — the UI doesn't clearly indicate the next action

**Don't Make Me Think** (Steve Krug): This is the right mantra. Not "reduce friction" — reduce cognition. Every moment where a user has to make a decision has a metabolic cost (literal glucose use, literal ATP synthesis). Worse, if they make a decision they don't understand, they feel stupid. That emotional association sticks to the product.

The Snapchat teenager: tapping 4-6 times per second on a jetway, fluently navigating a complex interface. Not fewer taps — more taps, but each trivially easy. If you'd tried to reduce her taps, you'd have ruined the experience. The goal is trivially easy decisions, not fewer decisions.

The Uber early app: "Where would you like to go?" and "Other." Everything else was behind Other. Perfect. Not fewer taps to accomplish a specific action — the most common action immediately presented, everything else deprioritized.

---

### Owner's Delusion — The Founder Bias Trap

Named by a Twitter user who has since deleted their account; Butterfield popularized it.

The restaurant website problem: Five things anyone ever wants from a restaurant website — address, phone number, menu, hours, reservation link. What restaurant websites actually deliver: slow-loading Ken Burns effect photo, Flash animation, music autoplay, and a non-clickable image of the phone number.

The restaurant owner has been to other restaurants and wanted those five things. So why does their own website not have them? Owner's Delusion: the owner sees their product through the lens of their investment in it, their vision of it, their pride in it. They don't see it as a stranger with low intent who just wants the phone number.

The Apple Sleep example: iOS Clock app has a feature called "Sleep." The description: "In order to automatically turn on sleep features and edit your schedule, you need to turn sleep on." Stewart still doesn't know what turning sleep on does. 98% of users probably don't either. Someone spent enormous effort building this feature. No one benefits because comprehension failed.

**The cure**: Take a breath. Pretend you're a regular person. Look at the thing. Can you figure out what it's supposed to do? What action you're supposed to take? What will happen if you take that action?

---

### Hyper-Realistic Work-Like Activities and Known Valuable Work

See [Hyper-Realistic Work-Like Activities](../concepts/hyper-realistic-work-like-activities.md) for the full framework.

The short version: as organizations grow, the supply of **known valuable work** (work you know what it is AND know it's valuable) decreases while the headcount doing work increases. The gap fills with work that *looks* like work — meetings to preview decks, meetings about meetings, A/B tests of features that couldn't possibly move the needle — but produces no value.

The Slack threads example: the input box for thread replies was pre-populated with @[previous_poster]. Butterfield removed it because (a) nobody wants to start their sentence with an @, and (b) it teaches users the wrong thing (they already get notifications automatically). Six months later it came back, backed by A/B test data showing threads were 2.17 messages long with the feature vs. 2.14 without.

The cost of generating that finding: feature flags, instrumentation, database tables, query writing, dashboards, multiple meetings including a rescheduled one. Thousands of person-hours. The maximum possible benefit from having this feature: essentially zero. Guaranteed net negative. This is a textbook HRWLA.

**Parkinson's Law** (1955, The Economist): Work expands to fill the time available for its completion. In an org context: every PM wants to hire someone to "do the product management so I can do strategy." Not because they're evil or stupid — because everyone knows headcount correlates with career trajectory, salary, and authority. The organization naturally grows beyond its known-valuable-work supply and the gap fills with HRWLA.

The leader's responsibility: ensure sufficient clarity around known-valuable work, say no explicitly upfront, don't let ambiguity become the petri dish for HRWLA.

---

### Tilt Your Umbrella — Empathy as Competitive Advantage

Walking back to the Vancouver office in rain, narrow Yaletown sidewalks, umbrellas at eye level. About one-third of people tilt their umbrella so you can pass. Two-thirds don't.

Three explanations for not tilting:
1. A tiny fraction: actually want to dominate
2. A larger fraction: see the problem, can't think of a solution
3. The majority: completely oblivious to their impact on others

"Your failure to really exercise this courtesy and be empathic about other people's experience is an advantage." Most companies don't notice how they're poking people in the eye. Their failure to notice is your opening.

Slack's word-of-mouth growth was driven by this: person leaves startup A for startup B, startup B doesn't use Slack, and they genuinely advocate for it — "Oh my God, you guys, you really have to try this." The emotional connection from small moments of empathy (the shouty rooster, magic links, DnD rollout) is what drove organic spread.

"Tilt your umbrella" became a Slack company value, printed on swag.

---

### Product Craft Details — Specific Slack Examples

**Magic links**: Why ask for email + password if the email ownership was the proof? Just send a link. Also solved the mobile problem of typing complex passwords on a phone. Butterfield credits someone else with the invention; Slack scaled it first.

**Notification defaults for new accounts**: First instinct was "only notify for DMs and @mentions." But new users need to understand the product works. Solution: send notifications for all messages by default, then after 10 messages received, show a prompt offering to switch to recommended settings. Worth the investment to get people through the onboarding hump.

**The shouty rooster** (@everyone): @everyone abuse was a tragedy of the commons — each person's message seemed important so everyone used it. Solution: show a rooster with sound waves when you @everyone, with a "This will notify 147 people in 8 time zones. Are you sure?" message. Drop-off was immediate. Trivially easy to implement, made a big difference, and educated users about the feature simultaneously.

**Do Not Disturb rollout** (2017): Tens of thousands of paying customers, operations alerts going to on-call channels for some of the world's largest systems. Can't just deploy. Solution: notify all Slack admins weeks before launch, set a default (7pm–7am) that they can override, which individual users can then override, which admins can re-override when needed. Elaborate, but it preserved the existing setups that people relied on and ensured the default got set (most people would never set it themselves).

---

### "We Don't Sell Saddles Here" — Origin Story

See [We Don't Sell Saddles Here](../concepts/we-dont-sell-saddles-here.md) for the full concept.

Written as an internal memo when Slack was 8–10 people, before the public launch, during private beta. Purpose: instill the ideas as early as possible so they could survive the scaling. Not edited before being made public — the version that circulated was verbatim what he wrote internally.

Butterfield credits the underlying idea to advertising and marketing practice ("if you want to sell Harley-Davidson, you're selling the open road"), but the product application — that you are "not just creating the product but also creating the market" — was his synthesis.

*Positioning* (Ries & Trout, 1981): Almost impossible to create a new idea in someone's head. Easier to take two existing ideas and combine them. "It's like Jaws meets Star Wars." If your product is different from alternatives in any significant way, you're not just building the product — you're building the category. Those are inseparable.

---

### Pivot Framework

"Have you exhausted the possibilities?" — the real question. Not "is this hard?" but "have I tried all the realistic good ideas?"

Glitch → Slack: By the point of the pivot, $9M still in the bank, everyone liked the game, still happy. But Butterfield had exhausted every non-ridiculous long-shot idea to make it commercially successful. The proto-Slack (started as IRC for internal communication) had been built organically, only adding features that were so obviously needed they couldn't not be built. Years of unintentional product development without the distorting pressure of having to justify it.

**The emotional problem with pivoting**: It's "fucking humiliating." You convinced investors, early employees, press, and users. You made promises. People moved cities for the job. When you pivot, the community you built disappears. You have to admit publicly that you were wrong. Most founders keep going not because it's rational but because pivoting is too painful. The right call requires **cold rationality** — creating distance from the emotional weight of having committed to the thing.

Annie Duke's *Quit* (second book after *Thinking in Bets*): Uses Glitch→Slack as an example of a smart fold. When expected value drops below the next best alternative, the rational choice is to fold even when that feels like failure.

---

### Value Creation as Company Chant

At multiple company all-hands, Butterfield had the entire company repeat:

> *"In the long run, the measure of our success will be the amount of value that we create for customers."*

Not "value we demonstrate" — value we **actually create**. If anything feels slightly shady, like you're maximizing at the customer's expense or taking advantage — don't. Not just because it's ethical, but because it's strategically correct: you attract better employees, create an emotionally connected customer base, and build something that actually lasts.

Prisoner's dilemma framing: acts of generosity signal cooperation in an iterated game. Both sides benefit when they can trust the other won't defect. Butterfield saw his generosity (100% health insurance, employee-friendly IPO structure, automatic SLA credits, fair billing) through this lens — not altruism, but a rational strategy for building durable relationships.

The SLA story: "For any downtime, you get 100x your money back." Fine when revenue is small. After going public, a multi-hour outage triggered $8M in credits. Changed the terms after that. Found the edge of generosity.

---

## Notable Quotes

> "I feel like what we have right now is just a giant piece of shit. It's just terrible and we should be humiliated that we offer this to the public." — Butterfield to MIT Technology Review, 2014 (printed out and put on the wall)

> "If you can't see almost limitless opportunities to improve, then you shouldn't be designing the product."

> "In the long run, the measure of our success will be the amount of value that we create for customers."

> "Your margin is my opportunity." — Jeff Bezos (quoted by Butterfield); equivalently: "Your failure to exercise empathy is my opportunity."

> "It's fucking humiliating." — on the emotional reality of pivoting

---

## Frameworks Introduced

- [Utility Curves](../concepts/utility-curves.md) — S-curve of feature value; investment below/at/past the threshold
- [We Don't Sell Saddles Here](../concepts/we-dont-sell-saddles-here.md) — Position products by transformation enabled, not what they technically are
- [Hyper-Realistic Work-Like Activities](../concepts/hyper-realistic-work-like-activities.md) — Work that looks like work but produces no value; org dysfunction framework
- Owner's Delusion — Founders/PMs see their product through their investment, not through a stranger's eyes
- Comprehension vs. Friction — The real design challenge is usually comprehension, not friction
- Don't Make Me Think — Reduce cognition, not clicks
- Tilt Your Umbrella — Empathy as competitive advantage; noticing impact on others is the opening
- Parkinson's Law — Work expands to fill the time available; orgs grow past supply of known valuable work

---

## PM Relevance

1. **Utility Curves for roadmap prioritization**: For every feature in the Microsoft Copilot roadmap, ask: are we at the beginning of the curve (not enough investment to clear the value threshold), the steep middle (high ROI), or past the cliff (diminishing returns)? Most organizations over-invest in the flat end of existing features and under-invest in getting new features past the threshold.

2. **Comprehension over friction for Copilot onboarding**: Copilot's core challenge is not that sign-up is too long — it's that users don't know what to ask it for, can't predict what it'll do, and don't understand which context it has access to. That's a comprehension problem. "Don't Make Me Think" applied: the product should make the right action obvious without explanation. Every point of uncertainty is a user who bounces.

3. **Owner's Delusion at Senior Director level**: You've been close to the product long enough to have lost the stranger's perspective. Counter it structurally: require PMs to do cold-start usability sessions before roadmap reviews. Never demo your own product to stakeholders without having watched a new user use it recently.

4. **HRWLA as a team health metric**: If your PMs are spending significant time in review meetings, preview decks, and A/B tests of marginal features, that's a supply/demand mismatch. Your job as the leader is to create sufficient clarity around known valuable work. Explicitly killing low-signal work is a leadership act.

5. **Saddle positioning for Copilot briefings**: Every time a product review asks "what does this feature do?", that's a saddle answer. Retrain the room: "what does this change for the user?" If the team can't answer the transformation question, the feature isn't ready for the roadmap.

6. **Tilt your umbrella for cross-functional dynamics**: Most cross-functional friction at Microsoft (between product, engineering, legal, policy) is caused by organizations that are oblivious to their impact on the people downstream from them. The opportunity is to be the team that proactively tilts — gives early heads-up, makes things easy for partners, doesn't create work for others. That reputation compounds.

7. **The value creation chant for team culture**: "In the long run, the measure of our success will be the amount of value we create for customers." This is worth surfacing with your team explicitly. At Microsoft scale, the temptation to optimize for metrics, adoption numbers, or feature velocity is constant. The chant is a useful reset: does this actually make customers' lives better?

---

## Entities Mentioned

- [Stewart Butterfield](../entities/stewart-butterfield.md) — Co-founder, Slack and Flickr
