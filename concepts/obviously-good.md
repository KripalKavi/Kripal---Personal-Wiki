---
title: "Obviously Good"
type: concept
date_added: 2026-05-15
tags: [product-strategy, design, leadership, frameworks, microsoft-relevant]
sources: ["https://www.lennysnewsletter.com/p/why-cultivating-agency-matters-more"]
related: ["../podcasts/lenny-max-schoening-agency-over-skills.md", "../entities/max-schoening.md", "../concepts/tiny-core.md", "../concepts/first-ten-percent-free.md", "../concepts/utility-curves.md"]
---

# Obviously Good

## Definition

A product ships **obviously good** when no reasonable person, on first encounter, would argue it isn't good. Not "good enough." Not "shippable." Not "meets the bar." *Obviously* good — instantly recognized.

[Max Schoening](../entities/max-schoening.md) installed this as an internal Notion principle, written on stickers ("obviously good"):

> "Let's just only make obviously good stuff. The origin, which is like — okay, wait, what does that mean? And I'm like, 'Ah, you know it when you see it.' I don't think anyone argued when they saw the first iPhone that it's obviously good. I don't think anyone argued that when ChatGPT first came out that it's obviously good. And so I think that's the bar."

---

## Why It Matters

Most product organizations ship under a different bar — *"we agree this is acceptable to ship."* That bar is satisfied by committee. Obviously good cannot be satisfied by committee, because the test is whether *anyone* would argue against it on first encounter. If even one person honestly says *"this isn't good,"* you haven't cleared the bar.

This is harsher than it sounds. It eliminates:
- Features that are competent but undifferentiated
- Polish that aims for "fine" rather than "wow"
- Compromises stacked on compromises
- "Ship it, we'll iterate" used as cover for not having figured it out

The two canonical examples Schoening invokes — **the iPhone in 2007 and ChatGPT in 2022** — share a property: not "we made the next iteration of an existing thing well," but "we made a thing such that no one needed convincing."

---

## The Tension with Shipping Cadence

Obviously good appears to contradict velocity. Notion's other operating principle is **shots on goal** — ship lots of experiments, increase the experimental rate. Schoening reconciles the two via **incremental correctness**:

> "I think the mistake that maybe a lot of companies then make is: 'great, we're going to be in this cave in isolation until we have it be obviously good.' One of my core values is incremental correctness, which is iterate — get really, really good at iterating."

So: iterate fast, in public, with users, *toward* obviously good. Don't ship the not-yet-good and call it iterating. Don't hide in a cave waiting for perfection. The discipline is whether the iteration *trajectory* is converging on obviously good — and whether you have the honesty to recognize when it isn't.

---

## "You Know It When You See It" — Why That's Not a Cop-Out

The phrase looks like a punt, but Schoening is precise about why it isn't:

1. Obviously good is **recognized**, not **described**. You can rarely prove a thing is good in advance; you can almost always tell when you encounter it.
2. The recognizers must include *non-employees*. The internal sycophancy filter is what makes "I think this is good" useless and "no one is arguing against it" meaningful.
3. The opposite — obviously *not* good — is also recognized instantly. If a reviewer pauses to argue *why* it isn't good, you've already failed the test.

This connects to Schoening's working definition of [Taste](../podcasts/lenny-max-schoening-agency-over-skills.md): *"a virtual machine in your head where, given an idea, you can predict for a certain in-group whether they're going to like it or not."* Obviously good is the case where the prediction is unanimous.

---

## The Industry Quality Critique

Schoening uses Obviously Good to diagnose what AI hasn't fixed:

> "I do have a general issue with vibe coding in the sense of I don't feel like the quality of software has increased all that much in the last 12 months. I think maybe the amount of software has, but it's very, very hard to find software that is reliable."

> "I live in the CLIs, it's great. But a regression every two weeks of a thing that was fixed three weeks before, and they still can't render a TUI at a frame rate that's reasonable. And so I think quality is a thing that's missing — this Apple-esque machined, unibody-aluminum kind of engineering. I would like us to figure out how to get back to that as an industry."

The implication: [First 10% Is Free](../concepts/first-ten-percent-free.md) democratized demos but did not democratize obviously good. Obviously good is the new craft frontier.

---

## Related to Adjacent Concepts

- **[Tiny Core](../concepts/tiny-core.md)** — obviously good is what a tiny core feels like when it's right. iPhone multitouch *was* obviously good. Notion blocks *would have been* obviously good if the editor hadn't been so rough — and it didn't matter, because the core was strong enough.
- **[First 10% Is Free](../concepts/first-ten-percent-free.md)** — the first 10% is free; the obviously-good 10% is the last 10% (still 90% of the work).
- **[Utility Curves](../concepts/utility-curves.md)** — obviously good is *above the threshold* on Butterfield's utility S-curve. Below the threshold, no investment produces felt value.
- **Shots on goal** — the *quantity* discipline that pairs with obviously good's *quality* discipline.

---

## PM Application

For a Senior Director of PM at Microsoft:

1. **Use "obviously good" as a launch gate.** Replace the standard ship-readiness checklist with a single test: *"If we showed this to ten people without context, would any of them argue it isn't good?"* If yes, don't ship. (And reform the launch-readiness review to look like a candid first-encounter test, not a check of internal sign-offs.)

2. **Identify the cave-vs.-iteration trap.** Microsoft has both failure modes:
   - **Cave**: long internal incubation, ships with no real user contact (most enterprise features)
   - **Premature iteration**: ships demo-quality and calls subsequent fixes "iterating"
   The disciplined middle is iterating *in public*, with real users, on a trajectory toward obviously good. Audit which features are on that trajectory and which are on the wrong one.

3. **The Apple-unibody standard for Copilot.** Schoening explicitly names the bar as *"Apple-esque, machined, unibody-aluminum engineering."* Most current Copilot surfaces aren't there. Pick one surface — GitHub Copilot autocomplete is the closest example inside Microsoft — and treat it as the internal standard for what obviously good feels like.

4. **The lab self-roast applies inside Microsoft too.** Schoening: *"the labs are not exempt — a regression every two weeks of a thing that was fixed three weeks before."* Microsoft Copilot releases have similar regressions. The cultural move is to internalize that *quality regression is a brand event*, not a sprint event. Each regression of an Apple-esque polish degrades the obviously-good bar for the entire suite.

5. **Beware "good enough" as a Microsoft cultural reflex.** Microsoft has historically shipped at the "good enough for enterprise" bar. That bar may have been sustainable when the alternative was nothing. In a world where AI-native upstarts can ship the "obviously good" tiny-core experience faster, "good enough" is the slow path to displacement.

6. **Watch for sycophancy in product reviews.** Obviously good is fragile inside large orgs because internal reviewers want to be supportive. Specific intervention: invite an outsider (junior employee, customer, hostile peer) to the product review and have them be the obviously-good test. If they're not convinced, you don't ship.

---

## Sources

- [Lenny's Podcast — Max Schoening](../podcasts/lenny-max-schoening-agency-over-skills.md) — primary articulation, 2026-05-03 (Notion-internal sticker phrase)

## Related

- [Tiny Core](../concepts/tiny-core.md)
- [First 10% Is Free](../concepts/first-ten-percent-free.md)
- [Utility Curves](../concepts/utility-curves.md)
- [Naked Robotic Core](../concepts/naked-robotic-core.md)
