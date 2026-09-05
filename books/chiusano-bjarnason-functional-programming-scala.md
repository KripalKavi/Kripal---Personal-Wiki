---
title: "Functional Programming in Scala"
type: book
date_added: 2026-04-19
tags: [engineering, design, frameworks]
sources: ["Paul Chiusano & Rúnar Bjarnason, Functional Programming in Scala (Manning, 2014)"]
related: ["../podcasts/lenny-claude-code-boris-cherny.md", "../entities/boris-cherny.md"]
---

# Functional Programming in Scala

**Author**: Paul Chiusano & Rúnar Bjarnason
**Year**: 2014 (Manning Publications; known as "the red book")
**Recommended by**: Boris Cherny (Lenny's Podcast, 2026-02-19) — "The single best technical book I have ever read."

---

## Summary

The canonical text for rigorous functional programming, using Scala as the teaching language. The book derives the entire functional programming toolkit from first principles — pure functions, algebraic data types, monads, functors, parser combinators, IO handling — building up to a complete functional architecture. Boris Cherny calls it the book that shaped how he thinks about code, even now that AI writes all of it.

---

## Key Ideas

### Pure Functions and Referential Transparency
A pure function has no side effects and always returns the same output for the same input. This property — referential transparency — is what makes programs composable, testable, and easy to reason about. You can substitute the function with its result anywhere. This is not just a Scala property; it's a fundamental design principle that applies to any system.

### Thinking in Types
The type system is not a constraint — it's a specification language. A well-typed function signature tells you almost everything about what the function can do. The book trains you to design systems type-first: the types define the shape of the problem before you write any implementation. Boris describes this as "a way of thinking" he can't stop applying.

### Algebraic Data Types and Composability
Programs built from composable pieces — where each piece has a well-defined type contract — are predictably combinable. No hidden state, no surprising interactions. This is the design philosophy behind Claude Code's architecture: minimal scaffolding, well-defined interfaces, give the model tools and let it compose them.

### Monads as a Design Pattern
Monads (Option, Either, IO, State, etc.) are a generalized pattern for sequencing computations that carry extra context — failure, side effects, state. The book makes these accessible by deriving them from simpler primitives, showing that they're not a category theory mystery but a practical composability tool.

### Deriving Everything from First Principles
The most distinctive quality of the book: nothing is accepted on authority. Every abstraction is derived from simpler pieces. This approach trains a habit of mind: don't accept a pattern because it's conventional; understand why it works.

---

## Quotable Lines

Boris on the book:
> "It's very weird, because you're probably not going to use Scala. But there's this just elegance to functional programming and thinking in types, and this is just the way that I code, and the way that I can't stop thinking about coding."

> "You could think of it as a historical artifact. You could think of it as something that will level you up."

---

## PM Application

For a Senior Director of PM at Microsoft:

1. **The mental model, not the language**: Boris recommends this book explicitly for people who won't use Scala. The value is the thinking style — composability, type-first design, reasoning from first principles. These apply to product architecture decisions: a well-designed API, a well-specified data contract, or a well-typed evaluation rubric are all applications of this mindset.

2. **Understanding what makes AI-generated code good**: AI models like Claude produce better code in functional style, because pure functions are easier to reason about, easier to test, and less likely to have hidden interactions. Understanding functional principles helps you evaluate whether AI-generated code is well-structured, even if you don't write it yourself.

3. **Composability as a product design principle**: The functional principle — build composable pieces with clear contracts — maps directly to product architecture. Copilot features built as composable, independently-testable components are more maintainable and more testable (connects to the [AI Evals](../concepts/ai-evals.md) methodology) than features wired together with implicit dependencies.

4. **"Derive from first principles"**: Boris's praise of this book is specifically about the habit of mind it builds — not accepting patterns because they're conventional, but deriving from fundamentals. This is the same habit he applies to product decisions ("use common sense; think from first principles" was his life motto in the same episode).

---

## Related Books

- This is Boris's technical deep cut — a pairing with his own book *Programming TypeScript* (O'Reilly, 2019), which he mentions writing during a period when he "fell in love with the language itself"
