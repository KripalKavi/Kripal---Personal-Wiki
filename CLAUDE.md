# Wiki Schema

## Purpose
Personal knowledge wiki for a Senior Director of Product Management at Microsoft. Captures and synthesizes insights from podcasts, essays, articles, and other sources. Prioritizes actionable intelligence on: product strategy, AI/technology trends, growth frameworks, leadership, organizational design, and innovation.

**Editorial lens**: Filter for insights that are surprising, counterintuitive, or directly applicable to running large-scale product strategy at a major technology company. Skip surface-level observations.

## Directory Structure

```
Wiki/
├── CLAUDE.md              # This file — schema and conventions
├── index.md               # Content catalog (always read first when querying)
├── log.md                 # Append-only activity log
├── podcasts/              # Podcast episode summaries
├── essays/                # Essay and article summaries
├── books/                 # Book summaries
├── tools/                 # Software tools, repos, and apps studied as product artifacts
├── entities/              # People and company pages
├── concepts/              # Frameworks, ideas, and mental models
└── .claude/commands/      # Ingest, Query, Lint skills
```

## Page Formats

### Frontmatter (all pages)
```yaml
---
title: "Page Title"
type: podcast | essay | book | tool | entity-person | entity-company | concept
date_added: YYYY-MM-DD
tags: [tag1, tag2]
sources: ["url or citation"]
related: ["relative/path/to/page.md"]
---
```

### Podcast Page Structure
1. **Metadata**: Show, episode title, guest, host, date published, URL
2. **Summary**: 2-3 sentence episode overview
3. **Key Takeaways**: Bulleted insights, filtered for PM relevance
4. **Notable Quotes**: Direct quotes with context
5. **Frameworks Introduced**: Named concepts with brief definitions
6. **PM Relevance**: Explicit connection to product management practice
7. **Entities**: Links to entity pages mentioned
8. **Concepts**: Links to concept pages touched

### Essay/Article Page Structure
1. **Metadata**: Author, title, year, URL
2. **Summary**: Core argument in 2-3 sentences
3. **Key Ideas**: Major points with explanations
4. **Quotable Lines**: Memorable phrases worth reusing
5. **PM Application**: How these ideas apply to product management
6. **Related Concepts**: Links to concept pages

### Entity Page Structure (Person)
1. **Role/Background**: Current role and relevant history
2. **Key Ideas**: What they're known for thinking/saying
3. **Appearances**: Links to podcast/essay pages where they appear
4. **Relevance**: Why this person matters to follow

### Entity Page Structure (Company)
1. **What they do**: Core product and market position
2. **Growth story**: Key metrics and inflection points
3. **Strategic insights**: What their approach teaches
4. **Appearances**: Links to pages where they're discussed

### Concept Page Structure
1. **Definition**: What the concept means precisely
2. **Why it matters**: The insight behind it
3. **Examples**: Concrete illustrations
4. **PM Application**: How to apply it in practice
5. **Sources**: Where this came from
6. **Related**: Links to related concepts

### Tool Page Structure
For software tools, open-source repos, and apps captured as product artifacts (not as how-to docs).
1. **Metadata**: Author/maintainer, type (open-source repo, commercial product, etc.), source URL
2. **Summary**: 2-3 sentences — what it is AND what pattern it evidences (the wiki captures tools for product-strategy lessons, not as installation guides)
3. **Key Ideas**: The product/strategy patterns the tool reveals
4. **PM Application**: Explicit connection to product management practice at Microsoft
5. **Related Concepts**: Links to concept pages

## Conventions

- **Cross-references**: Use relative markdown links `[Page Name](../entities/name.md)`
- **Tags**: lowercase, hyphenated. Common tags: `growth`, `ai`, `product-strategy`, `leadership`, `org-design`, `activation`, `frameworks`, `microsoft-relevant`
- **Dates**: ISO 8601 (YYYY-MM-DD)
- **File names**: lowercase, hyphenated, descriptive (e.g., `anthropic-growth-amol-avasare.md`)
- **PM Relevance section**: Always include — this is the most important section for future queries. Be specific, not generic.

## Operations

See `.claude/commands/` for the three wiki skills:
- `/ingest` — Add a new source (URL or file)
- `/query` — Ask a question against the wiki
- `/lint` — Health-check the wiki for issues
