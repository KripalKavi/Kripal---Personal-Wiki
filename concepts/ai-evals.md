---
title: "AI Evals"
type: concept
date_added: 2026-04-19
tags: [ai, evals, product-quality, ai-development, frameworks, methodology, microsoft-relevant]
sources: ["https://www.lennysnewsletter.com/p/why-ai-evals-are-the-hottest-new-skill"]
related: ["../podcasts/lenny-ai-evals-hamel-husain-shreya-shankar.md", "../entities/hamel-husain.md", "../entities/shreya-shankar.md"]
---

# AI Evals

---

## Definition

An **eval** (evaluation) is a systematic test that measures whether an AI system's outputs meet defined quality criteria. Evals replace gut-feel assessment ("this seems good") with repeatable, scalable measurement — running automatically against new model versions, prompts, or data to detect regressions and validate improvements.

Where unit tests check that code does what it's supposed to, evals check that an AI does what it's supposed to — including dimensions that are inherently subjective, like tone, helpfulness, and reasoning quality.

---

## Why It Matters

Without evals, AI product quality is assessed by whoever looks at it most recently — which means it drifts, degrades, and surprises you in production. Evals make quality continuous and explicit.

The counterintuitive insight: writing evals is actually a requirements discipline. If you can't write a precise eval for a behavior, you haven't actually specified what you want. The act of building evals forces clarity that prose specs almost never achieve.

**Industry signal**: OpenAI's acquisition of Statsig (an experimentation and analytics platform) signals that eval infrastructure is now considered foundational infrastructure for AI companies — not an optional quality practice.

---

## The Eval Development Methodology

This is the methodology recommended by Hamel Husain and Shreya Shankar — the most rigorous PM-applicable process available:

### Step 1: Error Analysis (always first)
- Pull real user traces: actual inputs and outputs from your production system
- Manually read through them — not to categorize yet, just to observe
- This is the most important and most skipped step; intuitions about failure modes are usually wrong
- A "trace" = a complete interaction record: user input, system response, and ideally any intermediate steps

### Step 2: Open Coding
- Go through traces and tag raw failure modes as you encounter them
- No pre-existing categories — just labels for what you see
- Examples: "missed user intent," "correct answer but wrong format," "hallucinated citation," "too verbose," "ignored constraint in system prompt"
- Capture the actual examples alongside the tags — you'll need them later

### Step 3: Axial Coding
- Group your raw tags into 5–6 higher-level failure categories
- These categories represent the core failure dimensions for *your specific product*
- Example output for a summarization product: (1) factual errors, (2) omitted key information, (3) incorrect tone, (4) format violations, (5) scope errors
- This taxonomy becomes the backbone of your eval suite

### Step 4: Theoretical Saturation
- Continue coding new traces until no new failure types emerge
- This is your signal that you've adequately covered the failure space
- Premature saturation (stopping too early) leads to blind spots in your evals

### Step 5: Write the Evals
- Now, and only now, write evals targeting each failure category
- Each eval should have: a test case (input), the criterion being tested, and a pass/fail definition
- Use the real traces you collected as test cases — they represent actual user behavior

### Step 6: Choose Eval Type Per Criterion
- **Code-based evals**: For hard constraints and verifiable properties
  - Is the response under 200 words?
  - Does it contain a citation?
  - Is the output valid JSON?
  - Fast, deterministic, cheap to run
- **LLM-as-judge**: For quality dimensions that require interpretation
  - Is this response helpful?
  - Does it match the expected tone?
  - Is this reasoning sound?
  - Requires calibration: validate the judge's ratings against human judgments on a sample before trusting it at scale

### Ongoing: The Benevolent Dictator
- Assign one person to own the eval suite for a product area
- They make the judgment calls when coding is ambiguous and when calibrating LLM-as-judge prompts
- Without a single owner, different people's interpretations of quality contaminate the evals and make them unreliable

---

## Evals as PRDs

Coined by Brendan Foody: **eval prompts are living product requirements documents**.

The logic:
- A traditional PRD describes what a feature should do in prose
- An eval describes it in terms of what "success" looks like in a testable, repeatable form
- Prose specs are often ambiguous enough that two engineers implement the same requirement differently
- Eval criteria force you to resolve that ambiguity upfront

**Practical application**: Write your eval criteria before writing your feature spec. If you can articulate exactly how you'd test whether the AI behavior is correct, you've already written your requirements. If you can't, you haven't scoped the feature yet.

---

## Examples

- **Copilot summarization**: Evals test whether meeting summaries include the key decisions (factual coverage), don't attribute statements to the wrong person (factual accuracy), and match the requested length (format compliance)
- **Copilot code generation**: Evals test whether suggested code compiles (code-based), passes the user's existing tests (code-based), and matches the style conventions of the surrounding code (LLM-as-judge)
- **Customer support AI**: Evals test whether the response resolves the stated issue (LLM-as-judge), doesn't make promises the company can't keep (code-based rule), and matches brand tone (LLM-as-judge)

---

## PM Application

For a Senior Director of PM at Microsoft building AI products:

1. **Make evals a launch gate**: No AI feature ships without a defined eval suite. The eval criteria are the acceptance criteria. This is a process change that moves quality left — catching issues before users see them.

2. **Own the error taxonomy**: The open/axial coding step is product research, not engineering. PMs should lead this: read the traces, name the failure categories, and build the taxonomy. This is the most PM-valuable step in the entire process.

3. **Write evals before specs**: Use the "evals as PRDs" insight literally. Start feature scoping by asking: "How would I evaluate whether this AI behavior is correct?" The answer is your spec.

4. **Calibrate LLM-as-judge against your team's standards**: When using LLM-as-judge, have your team rate a sample of outputs, then validate whether the judge agrees. Disagreement reveals where your quality criteria are ambiguous — which is itself valuable.

5. **Assign eval ownership per product area**: Apply the Benevolent Dictator principle. Each product area (e.g., Copilot in Word, Copilot in Teams, GitHub Copilot chat) should have one PM or tech lead who owns the eval suite and its consistency.

6. **Use ~30 min/week ongoing**: Once the initial error taxonomy and eval suite are built, maintenance is low. This is achievable. The barrier is not time — it's the upfront investment of doing the error analysis rigorously.

---

## Sources

- [Lenny's Podcast — Why AI Evals Are the Hottest New Skill](../podcasts/lenny-ai-evals-hamel-husain-shreya-shankar.md) (Hamel Husain & Shreya Shankar, 2025-09-25)
