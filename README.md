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

## Reference material

`references/` holds the source material the skill draws on:

| File | Source | Covers |
| --- | --- | --- |
| `style-guide.md` | *The ACS Style Guide*, 3rd ed. (ACS/Oxford, 2006), ch. 9, 10, 15–17 | Grammar, punctuation, editorial style, figures, tables, chemical structures |
| `tone-examples.md` | 3 published JACS papers | Annotated tone/rhetoric excerpts |
| `document-structure.md` | Same 3 JACS papers | Observed section order and numbering conventions |
| `citation-format.md` | `american-chemical-society.csl` + 2 of the JACS papers' reference lists | In-text and reference-list citation formatting, by source type |
| `american-chemical-society.csl` | Zotero Style Repository, "ACS Guide 2026 revision" | The authoritative, machine-readable citation style `citation-format.md` is translated from |
| `NEEDED.md` | — | What's been incorporated and what's still open |

These are living documents. Known gaps are noted inline (see `NEEDED.md`);
the reference-set is JACS-derived, so a different target ACS journal's own
Instructions for Authors may need to be supplied for the document-structure
guidance to fully apply.

## Using this skill

Point Claude at this repository (or install it as a skill) and ask it to
write, revise, or format chemistry manuscript text — an abstract, an
introduction, a results/discussion section, or a reference list. Claude
will read the relevant reference file(s) before editing and flag any
stylistic judgment calls it makes along the way, rather than silently
rewriting.
