# ACS_Style

A Claude skill for writing and revising chemistry manuscript text to match
American Chemical Society (ACS) journal conventions: tone, prose/style,
document structure, and author-number (numbered, superscript) citations.

See [`SKILL.md`](./SKILL.md) for the full instructions Claude follows.

## What it does

- **Tone** — revises prose toward the formal, mechanism-forward,
  argumentative register typical of ACS-published papers (gap-statement
  openings, causal chaining tied to evidence, calibrated hedging, inline
  figure/table citation).
- **Prose/style** — applies ACS Style Guide rules for grammar, punctuation,
  hyphenation, capitalization, italics, and abbreviation discipline.
- **Document structure** — checks section order (Abstract, Introduction,
  Results and Discussion, Conclusion, Associated Content, Author
  Information, Acknowledgments, References) and figure/table/scheme
  numbering conventions.
- **Citations** — formats or checks in-text superscript numbering and
  reference-list entries for every common source type (journal article,
  book, thesis, patent, chapter/conference paper, website, dataset),
  per the official ACS numeric CSL style.

## Using this skill

Point Claude at this repository (or install it as a skill) and ask it to
write, revise, or format chemistry manuscript text — an abstract, an
introduction, a results/discussion section, or a reference list. Claude
will read the relevant reference file(s) before editing and flag any
stylistic judgment calls it makes along the way, rather than silently
rewriting.

## Using it with non-Claude agents

`SKILL.md` and the `references/*.md` files are plain markdown with no
Claude-specific dependencies, so any coding agent can use them:

- **Codex, Cursor, or similar** — see [`AGENTS.md`](./AGENTS.md), which
  points these agents at `SKILL.md` and the relevant reference file for a
  given task, following the same `AGENTS.md` convention those tools already
  read automatically.
- **Anything else** — paste `SKILL.md` plus the specific `references/*.md`
  file(s) the task needs into the agent's context or system prompt
  directly. The workflow and rules apply as written regardless of which
  model or tool is running it.

A portable `.skill`/`.zip` archive of this repo (for dropping into another
project or agent) can be built by zipping the folder as-is — see the repo's
commit history for one built this way, or ask Claude to rebuild it.
