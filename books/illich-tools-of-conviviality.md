---
title: "Tools for Conviviality"
type: book
date_added: 2026-05-15
tags: [design, product-strategy, frameworks, microsoft-relevant, leadership]
sources: ["Ivan Illich, Tools for Conviviality (1973)"]
related: ["../podcasts/lenny-max-schoening-agency-over-skills.md", "../entities/max-schoening.md", "../concepts/malleable-software.md", "../concepts/cultivating-agency.md"]
---

# Tools for Conviviality

**Author**: Ivan Illich
**Year**: 1973
**Recommended by**: [Max Schoening](../entities/max-schoening.md) (Lenny's Podcast, 2026-05-03) — "a weird one"

---

## Why Schoening Recommends It

> "It's the contrast between, you look at the history of technology and tools that let users exercise human ingenuity and autonomy versus tools that are more at industrial scale that almost have become destructive to human autonomy."

Schoening calls it "a weird one" because Illich is not a tech-industry author and the book predates personal computing entirely. But it is the deep canonical text for his belief in [Malleable Software](../concepts/malleable-software.md). The taxonomy — **convivial tools** vs. **industrial tools** — directly informs what kinds of products Schoening thinks deserve to exist.

---

## Summary

Illich (radical Austrian social critic, ex-Catholic priest) argues that tools and institutions cross a threshold beyond which they stop serving human autonomy and start dominating it. Below the threshold, a tool *amplifies* what people can do; above the threshold, the tool *takes over*, dictating behavior, requiring servicing, accumulating its own logic and overhead. He calls the lower regime **conviviality** — tools that invite shared mastery — and the upper regime **industrial scale** — tools that produce dependency.

His examples are pre-tech: medicine, schools, transportation, manufacturing. His thesis: in each domain, society has crossed thresholds that produce diminishing or negative returns to human flourishing — more iatrogenic illness from medical systems, more functional illiteracy from schools, more time spent in service of cars than saved by them.

The book is a manifesto for **deliberate threshold-keeping** — designing tools and institutions that stay below the conviviality limit, even when scale temptations push beyond.

---

## Key Ideas

### Convivial Tools

A convivial tool is one that:
- Can be mastered by a normal person without specialized credentialing
- Serves the user's purposes, not the tool-system's
- Can be put down and picked up by anyone
- Composes with other tools without locking users in
- Allows users to shape outcomes, not just consume defaults

Examples Illich gives: hand tools, bicycles, libraries, small-scale workshops.

### Industrial Tools

An industrial tool is one that:
- Requires extensive specialization to operate
- Imposes its own logic on the user (you adapt to it, not it to you)
- Produces dependency — users cannot live without it
- Concentrates power in those who maintain it
- Accumulates externalities that exceed its benefits past a threshold

Examples Illich gives: hospitals as institutional systems, the school-as-credentialing-machine, automobile-centric urban design.

### The Conviviality Threshold

The provocation: every tool can be convivial below a certain scale and industrial above it. The same tool flips. Medicine performs healing below a threshold; above, it manufactures illness. Education enables learning below a threshold; above, it manufactures functional illiteracy. The work of a good society is to *find and respect* those thresholds — not to maximize.

### Counter-productivity

Once a tool is past its conviviality threshold, *more of it produces less of the benefit it claims to provide.* This is Illich's most striking empirical claim: doubling the medical system does not double health. Doubling the school system does not double literacy. Doubling roads does not double transportation. The tool has become its own end.

---

## Why This Applies to AI Products in 2026

Schoening's implicit reading: most current SaaS sits firmly in the industrial regime (vendor-controlled, dependency-creating, dictates workflow). [Malleable Software](../concepts/malleable-software.md) is an attempt to drag software back toward conviviality:

- User shapes the tool to their work, not vice versa
- Composable without lock-in
- Mastery accessible without specialist credentials
- Generative substrate, not glued-shut app

AI is the most powerful conviviality-amplifier yet — *if* it's deployed as a substrate-for-making rather than as another industrial layer. The risk: AI products that maximize platform lock-in, opacity, and user-as-consumer dynamics become Illich's worst case — industrial tools that produce dependency at unprecedented scale.

The personal-AI-agent pattern (see [OpenClaw](../essays/lenny-claire-vo-openclaw-personal-ai-agent.md)) is an explicit Illich-flavored move: build your own agent so you keep the conviviality.

---

## PM Application

For a Senior Director of PM at Microsoft:

1. **Conviviality as a product-design lens.** Apply Illich's test to any Microsoft product: *Does this tool serve the user's purposes or its own? Does it create dependency or capability? Can a user master it without becoming a specialist?* Most enterprise software fails these tests. Copilot has an opportunity to be the convivial layer *on top of* the industrial substrate.

2. **The dependency anti-pattern is a real risk for Copilot.** A Copilot that does the user's work *for* them risks Illich's counter-productivity: more Copilot → less human capability. A Copilot that helps users *do* their work — and learn while doing — stays convivial. The framing matters in product design and in marketing.

3. **The "industrial AI" failure mode.** Big Tech AI products tend to centralize: closed weights, opaque reasoning, vendor-controlled context, no user-side composition. This is industrial in Illich's sense. Microsoft can position differently: model-agnostic Copilot, user-owned context (Graph), composable agent SDK, transparent reasoning where possible. This is a *philosophical* differentiation, not just a feature one.

4. **Read alongside Code (Petzold).** Petzold gives the substrate fluency; Illich gives the substrate values. The pair argues for AI products that respect both *how things work* and *what tools should do for humans.*

5. **Counter-productivity audit for Microsoft tools.** Are there Microsoft products that pass Illich's "more of it produces less of what it claims" test? Probably some collaboration tooling (Teams notifications, meeting tooling). Worth thinking about deliberately.

---

## Related Concepts

- [Malleable Software](../concepts/malleable-software.md) — the direct application of Illich's conviviality to software design
- [Cultivating Agency](../concepts/cultivating-agency.md) — the user-side counterpart: tools should make humans more capable, not more dependent
- [Harness as Moat](../concepts/harness-as-moat.md) — the harness can be convivial (composable substrate) or industrial (closed platform); the strategic choice matters
