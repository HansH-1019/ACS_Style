# Status: what's supplied vs. still open

## Supplied and incorporated
- ACS Style Guide (3rd ed.) chapters 9, 10, 15, 16, 17 → `style-guide.md`
- 3 published ACS papers (tone source) → excerpts + patterns in `tone-examples.md`
- `american-chemical-society.csl` (Zotero/CSL "ACS Guide 2026 revision",
  numeric in-text style) → authoritative reference-list rules for every
  type (journal article, book, thesis, patent, chapter/conference paper,
  webpage, and a generic fallback) in `citation-format.md`, cross-checked
  against the two JACS papers' real reference lists (exact match).
- Same 3 papers' section order → `document-structure.md`

## Still open
- `document-structure.md`: section order is JACS-specific; a different
  target ACS journal (Org. Lett., Anal. Chem., ACS Nano, etc.) may differ.
  Paste that journal's own Instructions for Authors if this matters for the
  manuscript at hand.
- Citation formatting is now resolved for essentially every source type via
  the CSL file — no open gap there.
