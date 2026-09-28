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
