Health-check the personal knowledge wiki.

## Context

This wiki belongs to a Senior Director of PM at Microsoft. It is designed to compound value over time — but only if pages are well-connected, current, and high-quality. Run this periodically (suggested: monthly) to catch drift.

## Instructions

**Step 1 — Read `index.md` and `log.md`**
Get a full inventory of pages and activity history. Note: when was the last ingest? Are there recent ingests that might have created pages without updating the index?

**Step 2 — Scan all content directories**
Read all pages in `podcasts/`, `essays/`, `entities/`, `concepts/`. Note which files exist on disk vs. which are listed in `index.md`.

**Step 3 — Check for issues**

**Structural issues** (fix immediately):
- Orphan pages: Pages that exist on disk but are not listed in `index.md`
- Dead links: Internal links pointing to files that don't exist
- Missing frontmatter: Pages without required YAML frontmatter fields (title, type, date_added, tags, sources, related)
- Missing required sections: Podcast/essay pages without a "PM Relevance" section; concept pages without a "PM Application" section

**Content quality issues** (flag for review):
- Generic PM Relevance: Sections that say things like "useful for product thinking" without specific application
- Contradictions: Claims on one page that conflict with claims on another
- Stale content: Pages referencing fast-moving topics (AI capabilities, company metrics) added more than 6 months ago — may need updating
- Duplicate content: Substantially the same insight captured in multiple places without cross-linking

**Coverage gaps** (suggest for ingestion):
- Entity pages referenced in source pages but not yet created
- Concept pages referenced but not yet created
- Topics that appear frequently across pages but lack a dedicated concept page
- Index Topic Index entries that are incomplete or missing categories

**Step 4 — Report findings**
Structure the report as:

```
## Lint Report — [DATE]

### High Severity (fix now)
1. [Issue description + specific file]

### Medium Severity (flag for review)
1. [Issue description + specific file]

### Low Severity (optional improvements)
1. [Issue description + specific file]

### Coverage Gaps (suggested ingestions)
- [Topic/source suggestion]
```

**Step 5 — Fix high-severity issues**
Fix these without asking:
- Add missing orphan pages to `index.md`
- Fix dead internal links (update to correct path or remove)
- Add missing frontmatter stubs
- Create empty stub pages for referenced-but-missing entity/concept pages with a `stub: true` frontmatter flag

Do NOT auto-fix medium or low severity issues — flag them for the user's review.

**Step 6 — Append to `log.md`**
`[YYYY-MM-DD] LINT [N issues found: X high, Y medium, Z low. Fixed: [summary]. Remaining: [summary of unfixed issues].]`

**Step 7 — Report to the user**
Summary of what was found, what was fixed, and what needs attention.
