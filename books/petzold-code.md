---
title: "Code: The Hidden Language of Computer Hardware and Software"
type: book
date_added: 2026-05-15
tags: [engineering, design, frameworks, microsoft-relevant]
sources: ["Charles Petzold, Code (1999; 2nd ed. 2022)"]
related: ["../podcasts/lenny-max-schoening-agency-over-skills.md", "../entities/max-schoening.md", "../concepts/cultivating-agency.md", "../concepts/malleable-software.md"]
---

# Code: The Hidden Language of Computer Hardware and Software

**Author**: Charles Petzold
**Year**: 1999 (first edition); expanded 2nd edition 2022
**Recommended by**: [Max Schoening](../entities/max-schoening.md) (Lenny's Podcast, 2026-05-03)

---

## Why Schoening Recommends It

> "Do you know how computers actually work? It is actually surprising to me how many professionally employed programmers don't know how computers work. That one — the funny thing is, it does not have a line of code in it until chapter 27. So exceptionally good book."

The recommendation is targeted: in an era when the abstraction layer above hardware is becoming dominated by LLMs and natural-language interfaces, fewer practitioners understand the substrate. Petzold's book is a *substrate education* — Morse code, Braille, electrical relays, logic gates, memory, CPU architecture — built from first principles without any actual code until chapter 27. By the time code appears, the reader has already built a computer in their head.

For Schoening, this is part of the **cultivate agency through making + understanding substrate** worldview. You can't reshape what you don't understand. The terminal vs. GUI preference at Notion is the same instinct: get people closer to the material.

---

## Summary

Petzold builds the entire concept of a computer from the absolute ground up — starting with two children flashing flashlights between bedroom windows and ending with a programmable CPU running real software. Each step is small enough that no prior computer-science knowledge is required, but rigorous enough that the abstractions stay grounded in physical mechanism.

The chapters layer:
1. **Codes** — Morse, Braille, the conceptual idea that meaning can ride on symbols
2. **Electricity and relays** — physical mechanisms that can perform logic
3. **Boolean logic + gates** — combining relays into logical operations
4. **Memory** — feedback loops that store state
5. **Arithmetic** — building adders, then multipliers, then ALUs
6. **The CPU** — putting it all together into an executable architecture
7. **Languages and operating systems** — the abstraction layers above
8. **Modern computing** — extended in the 2022 edition to cover modern processors, the web, etc.

The 2022 second edition expands and modernizes substantial portions, especially around modern CPUs and the web.

---

## PM Application

For a Senior Director of PM at Microsoft:

1. **Make Code a recommended reading for AI-era PMs.** Most current PMs (Schoening's claim, broadly true at Microsoft) work at very high abstraction layers. When they reason about AI products, they reason about prompts and outputs, not about what the model is *doing*. Building substrate intuition — even at a relay/gate level — produces better judgment about what AI can and can't do. Petzold's book is the most efficient way to get that intuition without a CS degree.

2. **The PM-can't-debug-anything pattern.** When something goes wrong with a Copilot feature, the PM who can hypothesize *why* (latency? context window? tool use loop? memory? RAG?) is more valuable than one who can only describe the symptom. Substrate fluency compounds across every AI product decision.

3. **Pair with Schoening's "designers should code" thesis.** Both moves push product people closer to the medium. Code is the long-form, structured version of the same instinct: don't be the cog at the top of the stack who only sees outputs.

4. **The 2022 expansion covers AI substrate.** Worth specifically referencing if the team is building AI products — the second edition's modern-computing chapters give just enough hardware-and-systems grounding to make the AI stack legible (why latency is what it is, what GPUs actually do, what memory bandwidth means in practice).

---

## Quotable Setup

The book famously does not contain a line of code until chapter 27 — Schoening calls this out specifically. The point: you don't need code to understand computers; you need to understand computers to write code well.

---

## Related Concepts

- [Cultivating Agency](../concepts/cultivating-agency.md) — substrate understanding is what makes the world legibly malleable
- [Malleable Software](../concepts/malleable-software.md) — you can't reshape what you don't understand
