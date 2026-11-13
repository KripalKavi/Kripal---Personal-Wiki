---
title: "Obsidian Claude Sidebar: Multi-Backend Agent Harness in a Notes App"
type: tool
date_added: 2026-05-11
tags: [ai, agentic-ai, product-strategy, microsoft-relevant, developer-tools, workflows]
sources: ["https://github.com/derek-larson14/obsidian-claude-sidebar"]
related: ["../concepts/harness-as-moat.md", "../concepts/model-eats-the-harness.md", "../essays/lenny-claire-vo-openclaw-personal-ai-agent.md"]
---

# Obsidian Claude Sidebar: Multi-Backend Agent Harness in a Notes App

**Author**: Derek Larson
**Type**: Open-source project (Obsidian community plugin), ~395 stars, MIT license
**Source**: https://github.com/derek-larson14/obsidian-claude-sidebar

---

## Summary

A community-built Obsidian plugin that embeds a full pseudo-terminal running Claude Code (or one of seven interchangeable AI coding backends) directly in the notes app's sidebar. The interesting part is not the plugin itself — it is what the plugin reveals: at the workspace UX layer, AI coding agents are already being treated as commodity, swappable backends, while the harness (sidebar, terminal emulator, file/folder context, permission model, multi-session tabs) is becoming the durable product surface.

---

## Key Ideas

### 1. Models are commoditizing at the workspace UX layer

The plugin's settings let a user swap between **Claude Code, Codex, OpenCode, Gemini, Kimi Code, GitHub Copilot, and Pi** — all wired into the same sidebar, terminal, context menus, and file-path injection. From the user's seat, the model is a dropdown. The "agent in my workspace" experience is constant; the brain behind it is interchangeable.

This is the developer-tools microcosm of a broader pattern: as coding agents converge on similar capabilities (file edits, terminal access, planning, multi-step execution), the *workspace they live in* — not which lab's model is wired up — becomes the user's anchor.

### 2. The harness is the durable layer

What does this plugin actually provide that the underlying CLIs do not?

- **Surface**: Embedded sidebar always-on, not a separate window the user has to alt-tab to
- **Context plumbing**: Right-click a folder/file → launch Claude there or inject its path
- **Session management**: Multiple concurrent agent tabs (Claude Code does not natively do this in a single UI)
- **Terminal emulation**: xterm.js + Python `pty` / pywinpty, including WSL path translation on Windows
- **Permission UX**: A `--dangerously-skip-permissions` "YOLO mode" toggle exposed as first-class product surface
- **Onboarding**: One-line curl install, BRAT auto-updates

None of this is model work. All of it is the harness — and it survives Claude → Codex → Gemini → next-model swaps unchanged.

### 3. The "embed in existing tools" play vs. building a new destination

The plugin author did not build a new notes app or a new agent app. They embedded the agent into the notes app users already keep open. Compare:

- **Destination strategy**: Cursor, Windsurf, ChatGPT desktop — "switch to our app to use the agent."
- **Embed strategy**: This plugin, GitHub Copilot inside VS Code, Copilot in M365 apps — "the agent appears where you already are."

The embed strategy assumes the surface a user already lives in is more defensible than a new surface they have to be convinced to adopt.

### 4. The terminal is becoming a primary product surface for AI agents — even in non-developer tools

The author chose to embed an actual pseudo-terminal (with all the engineering cost that implies: xterm.js, pty handling, Windows-specific pywinpty, base64-embedded PTY scripts to satisfy Obsidian's plugin packaging) rather than build a chat UI on top of the API. The terminal is the agent's native surface. For the kinds of users who run Obsidian and run Claude Code, "give me the real terminal in a panel" beat "give me a polished chat wrapper."

---

## Quotable Observations

> "Switch between Claude Code, Codex, OpenCode, Gemini, Kimi Code, GitHub Copilot, and Pi."

A single sentence from the feature list that captures the commoditization thesis: seven agent backends, one sidebar.

> "Multiple Claude sessions concurrently in separate tabs."

The harness adds capability the underlying CLI does not have. Multi-session orchestration is becoming a workspace-level concern, not a model-vendor concern.

---

## PM Application

For a Senior Director of PM at Microsoft, three concrete implications:

1. **GitHub Copilot positioning vs. Cursor / Windsurf / Claude Code**: The competitive battle is increasingly at the workspace level, not the model level. Copilot's defensibility is "you are already in VS Code / Visual Studio / GitHub.com" — *the existing surface is the moat*. The risk: if a community plugin can wrap seven different agent backends behind a single workspace UX, then any sufficiently good workspace can swap GitHub Copilot out for a competitor's model. The strategic question is whether GitHub Copilot's value is the model (Anthropic / OpenAI provided) or the workspace integration (Microsoft built). Optimize the latter.

2. **Copilot in M365 surface strategy**: The plugin embeds the agent inside the tool the user already keeps open (Obsidian, in this case). This is the same play as Copilot in Word / Excel / Teams — *meet the user inside their existing workspace rather than asking them to context-switch to copilot.microsoft.com*. The plugin is independent validation that this strategy wins for power users. Implication: invest in deep, native, in-app Copilot surfaces over the standalone Copilot destination.

3. **Multi-backend agent abstraction as a forward indicator**: A plugin that lets users swap between seven AI backends is a leading signal that enterprise customers will demand the same. They will not want to commit to one model vendor at the workspace layer. Microsoft's existing posture here (Azure AI Foundry, model choice across providers in Copilot Studio) maps to this — but the user-facing manifestation matters: in M365 and GitHub Copilot, is there a clear story for "swap the model behind this experience"? If not, that is a product gap that competitors will exploit.

4. **Permission UX as first-class product surface**: The plugin exposes `--dangerously-skip-permissions` ("YOLO mode") as a settings toggle. That is a product design decision: agent permission models are not a backend detail, they are user-visible policy. For enterprise Copilot, the analog is whether tenant admins and end users have first-class, ergonomic controls over agent permissions — not buried in a JSON file, but as a real product surface. The community ergonomics here are ahead of where most enterprise products are.

---

## Related Concepts

- [Harness as Moat](../concepts/harness-as-moat.md) — The new concept this source most directly evidences: when models commoditize, the workspace harness becomes the durable layer
- [Model Eats the Harness](../concepts/model-eats-the-harness.md) — The inverse pattern at the *internal* product layer: prompt-engineering scaffolding gets eaten by better models. "Harness as moat" is about the *external workspace* harness; this is about the *internal compensatory* harness. Both are true; they operate at different layers.
- [OpenClaw / Claire Vo](../essays/lenny-claire-vo-openclaw-personal-ai-agent.md) — Parallel community-built personal AI infrastructure. Both sources show motivated power users assembling their own agent stacks from commodity components when commercial products do not meet their workflow needs.
