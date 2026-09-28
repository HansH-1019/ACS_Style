# AGENTS.md

Standing instructions for coding agents (Codex, Cursor, etc.) working in
this repository.

## What this repo is

`ACS_Style` is a Claude Agent Skill — a packaged set of instructions and
reference material for writing and revising chemistry manuscript text to
match American Chemical Society (ACS) journal conventions: tone,
prose/style, document structure, and author-number (numbered, superscript)
citations. It was originally built for Claude, but the content itself
(instructions + reference files) has no Claude-specific dependencies.

## When to use it

Before writing, revising, or formatting any chemistry manuscript text in
this repo or elsewhere — an abstract, an introduction, a results/discussion
section, a reference list, or a check of section/figure/citation
formatting against ACS conventions — read `SKILL.md` first. It lays out the
workflow (tone pass → prose/style pass → hedging calibration → structure
check → citation formatting) and links to the specific reference file each
step draws on:

- `references/style-guide.md` — ACS Style Guide grammar/punctuation/
  editorial-style rules and figure/table/chemical-structure conventions.
- `references/tone-examples.md` — annotated tone/rhetoric patterns from
  published ACS papers.
- `references/document-structure.md` — ACS article section order and
  numbering conventions.
- `references/citation-format.md` and `references/american-chemical-society.csl`
  — the numbered/superscript citation system and reference-list format,
  by source type.

## How to use it here

There's no special tooling required — `SKILL.md` and the `references/*.md`
files are plain markdown. Read `SKILL.md` in full before editing manuscript
text, then read only the specific reference file(s) the task at hand needs
(don't load all of them into context unless the task spans tone, structure,
and citations at once). Follow the workflow and "Explaining edits" section
in `SKILL.md` as written — it applies regardless of which agent is running
it.

If a rule needed for the task isn't covered by these files (see each file's
own "Still needed"/"Still open" notes, and `references/NEEDED.md`), say so
rather than inventing a plausible-looking ACS rule, and ask for one more
real source example instead of guessing.
