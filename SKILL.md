---
name: ACS_Style
description: >
  Revise, draft, or structure chemistry manuscript text to match American
  Chemical Society (ACS) journal conventions — formal, mechanism-forward
  academic tone; ACS Style Guide prose rules (word choice, sentence
  structure, abbreviations, units/numbers, hyphenation, figure/table/scheme
  conventions); standard ACS article section order (Abstract, Introduction,
  Results and Discussion, Conclusion, Associated Content, Author
  Information, Acknowledgments, References); and ACS author-number
  (numbered, superscript) in-text citations with matching reference-list
  formatting. Use this whenever the user asks to write, revise, polish,
  format, or "make this sound like ACS/JACS," for a chemistry manuscript,
  abstract, introduction, results/discussion section, or reference list —
  even if they don't explicitly say "ACS style." Also use it when asked to
  format citations/references for a chemistry paper in numbered style, or
  to check whether a draft's figure/table/scheme numbering and captions
  follow ACS conventions.
compatibility: none
---

# ACS_Style

Revise or draft chemistry manuscript prose so it reads like it belongs in
an ACS journal, and format its structure and citations to match. This
skill covers three layers — **tone**, **prose/style**, **document
structure** — plus **author-number citation formatting**. It does not cover
figure/graphic production itself, only how figures/schemes/tables should be
numbered, captioned, and referenced in prose.

## Reference files

Read the relevant file(s) before revising; don't try to hold all of this in
working memory from a summary.

- `references/style-guide.md` — ACS Style Guide (3rd ed.) chapters 9–10
  (grammar, punctuation, spelling, hyphenation, capitalization, italics,
  abbreviations) and 15–17 (figures, tables, chemical structures/schemes).
  This is the prose/style rulebook.
- `references/tone-examples.md` — annotated excerpts from three published
  ACS papers, each tagged with the rhetorical pattern it demonstrates
  (gap-statement openings, mechanism-forward causal chaining, calibrated
  hedging, inline figure citation, etc.). This is the tone model.
- `references/document-structure.md` — observed ACS article section order
  and figure/table/scheme numbering conventions.
- `references/citation-format.md` — the numbered/superscript in-text
  citation system and reference-list entry format for every source type
  (journal article, book, thesis, patent, chapter/conference paper,
  website, dataset/fallback), translated from `american-chemical-society.csl`
  (the authoritative CSL spec) and cross-checked against two real JACS
  reference lists.
- `references/american-chemical-society.csl` — the underlying CSL file
  itself. `citation-format.md` is the human-readable translation of it;
  consult the CSL directly for a field this skill hasn't needed yet, or if
  a citation-management tool needs the machine-readable style.

These files are living documents seeded from a limited set of sources (one
style-guide summary, three papers, one CSL file). If a rule is genuinely
missing — e.g., the target journal's specific section order differs from
the JACS-derived default in `document-structure.md` — say so rather than
inventing a plausible-looking rule, and ask the user for one more source
rather than guessing.

## Workflow

1. **Identify what's being asked.** A full manuscript section (Introduction,
   Results and Discussion, etc.), an abstract, a citation list, or a
   structural check (is this in the right section order, are figures
   numbered correctly)? The revision moves below apply mainly to prose;
   structure and citation checks are mechanical lookups against
   `document-structure.md` and `citation-format.md`.

2. **Revise prose in this order** (each pass should not undo the previous
   one — read the whole passage first, then edit):
   - **Tone pass** — against `tone-examples.md`'s checklist. Does the
     opening establish context before pivoting to the gap/novelty? Is the
     novelty claim stated plainly and early, scoped to what was actually
     shown? Are results narrated as a causal chain tied to specific
     evidence, not a flat list of observations? Is every figure/table cited
     inline, mid-sentence, where it's doing argumentative work — not just
     dropped in once?
   - **Prose/style pass** — against `style-guide.md` Chapters 9–10. Check
     subject-verb agreement past intervening phrases, restrictive vs.
     nonrestrictive clauses (*that* vs. *which*), introductory-modifier
     attachment, comma usage, hyphenation of compound modifiers, and
     abbreviation discipline (defined at first use, not redefined, not used
     for two different terms).
   - **Hedging calibration** — match the verb to the evidence: strong,
     direct evidence (X-ray, NMR, unambiguous spectroscopic assignment) gets
     strong verbs ("confirm," "demonstrate," "establish"); computational or
     indirect evidence gets calibrated verbs ("suggest," "is consistent
     with," "is reasonably assigned to"). Don't upgrade or downgrade the
     confidence level implied by the original draft's actual evidence —
     ask if it's unclear which the author means.

3. **Check structure** against `document-structure.md` when the task
   touches section order, headings, or where content belongs (e.g., "should
   this go in Results and Discussion or Conclusion?"). Check figure/
   table/scheme numbering and caption completeness against
   `style-guide.md` Chapters 15–17 (each numbering sequence is separate;
   captions must stand alone; every numbered item must be cited in text, in
   order).

4. **Format or check citations** against `citation-format.md` — superscript
   placement (no space, attached to the specific claim, not batched at
   sentence end), comma-separated multiples, en-dash ranges for 3+
   consecutive numbers, and the reference-list entry format (author
   semicolon list, sentence-case title, italicized abbreviated journal
   name, bold year, italicized volume, en-dash page range).

5. **When something isn't covered by the reference files**, don't
   improvise a rule that sounds plausible — say what's missing and, if it
   matters for the task at hand, ask the user for one more real example
   (a source citation of that type, a snippet of the target journal's
   author guidelines, etc.) rather than guessing. A wrong "ACS style" rule
   is worse than an honest gap, since the whole point is fidelity to the
   real convention.

## Explaining edits

When revising a passage, briefly flag *why* a nontrivial change was made
(which pattern or rule it follows), the way a copyeditor's comment would —
not a line-by-line diff essay, just enough that the author can tell a
stylistic judgment call from an error fix. Don't flag mechanical fixes
(obvious typos, hyphenation per Chapter 10) individually; do flag tone/
structure judgment calls (e.g., "moved the novelty statement earlier —
ACS abstracts front-load this rather than building up to it").

## What this skill does not do

- Does not generate or edit figures, schemes, or chemical structure
  drawings themselves — only their numbering, captions, and how they're
  cited in prose.
- Does not verify chemistry, data, or claims — only how they're expressed.
- Does not know a specific target journal's Instructions for Authors beyond
  what's in `document-structure.md` (JACS-derived) unless the user supplies
  that journal's guidelines.
