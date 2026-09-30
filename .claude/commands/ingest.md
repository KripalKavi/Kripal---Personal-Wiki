Ingest a new source into the personal knowledge wiki.

## Context

This wiki belongs to a Senior Director of Product Management at Microsoft. The editorial lens: capture insights that are surprising, counterintuitive, or directly actionable for large-scale product strategy at a major technology company. Skip surface-level observations.

## Instructions

You are adding a new source. The source URL or file path is provided as the argument to this command. If no argument is given, ask the user for the source.

**Step 1 — Read the source**
Fetch the URL or read the file. If the content is paywalled or inaccessible, tell the user and ask them to paste the content directly.

**Podcast transcript check (required for podcast sources):**
1. Search Podscripts (`podscripts.co`) using the exact show name and episode title to see whether a transcript exists.
2. Verify that the Podscripts result matches the exact episode title and publication date. Do not silently substitute a related, earlier, extended, or condensed episode.
3. If an exact transcript exists, use it as the primary transcript source and cross-check its title, date, description, and timestamps against the podcast's official episode page. Add both URLs to the page's `sources` frontmatter and identify the transcript used in Metadata.
4. Treat Podscripts transcripts as machine-generated: normalize only obvious transcription errors, keep direct quotations brief, and check technical terms, names, numbers, and surprising claims against the audio, official show notes, or primary sources when possible.
5. If only a related episode transcript exists, use it only as explicitly labeled background. Do not attribute its protocols, quotes, or details to the requested episode.
6. If no exact transcript is available on Podscripts, continue checking the official site and other reputable transcript sources. If the source remains paywalled or inaccessible, tell the user and ask them to paste or provide the content.

**Step 2 — Read the schema**
Read `CLAUDE.md` to confirm current wiki conventions and directory structure.

**Step 3 — Read the index**
Read `index.md` to understand what's already in the wiki. Avoid duplicating content that already exists — instead, add to existing pages where relevant.

**Step 4 — Brief discussion**
In 2-3 sentences, share your read on the most interesting or surprising insight in the source. Give the user a chance to redirect focus before you start writing.

**Step 5 — Create the primary page**
Choose the correct directory based on content type:
- Podcast episode → `podcasts/[slug].md`
- Essay or article → `essays/[slug].md`
- Book → `books/[slug].md`
- Video/talk → `talks/[slug].md`

File slug format: `[author-or-show]-[topic-keywords].md` (lowercase, hyphenated)

Follow the page format defined in CLAUDE.md for the content type. Always include:
- Frontmatter (title, type, date_added, tags, sources, related)
- A "PM Relevance" section — this is the most important section; make it specific, not generic

**Step 6 — Update or create entity pages**
For each person or company that appears prominently in the source, either:
- Update their existing page in `entities/` (add an appearance entry and any new key ideas), or
- Create a new entity page following the format in CLAUDE.md

**Step 7 — Update or create concept pages**
For each named framework or concept introduced in the source, either:
- Update an existing concept page in `concepts/` (add the new source as evidence), or
- Create a new concept page following the format in CLAUDE.md

**Step 8 — Update `index.md`**
Add the new pages to the appropriate table sections and the Topic Index at the bottom.

**Step 9 — Append to `log.md`**
Add a single log line in this format:
`[YYYY-MM-DD] INGEST [Source title and author]. Created: [list of new files]. Updated: [list of updated files].`

**Step 10 — Report to the user**
List which files were created and which were updated.

## Quality bar

- Capture only insights that are **surprising, counterintuitive, or directly actionable** for a Senior Director of PM at Microsoft
- PM Relevance sections must be specific — not "useful for product thinking" but "here's the specific application to Copilot onboarding / Copilot for M365 / Azure AI / team structure"
- Every page should pass: "Would I be glad I wrote this in 6 months?"
- Cross-reference aggressively — if a new concept connects to an existing one, link them in both directions
