# ACS Citation Format — Author-Number (Numbered) System

**Primary source:** `american-chemical-society.csl` in this directory — the
Zotero/CSL "ACS Guide 2026 revision" style (`citation-format="numeric"`,
`class="in-text"`). This is a machine-readable, authoritative spec; the
rules below are a human-readable translation of its logic, field by field.
Cross-checked against the real reference lists of the two JACS papers
supplied as tone references (`J. Am. Chem. Soc. 2021, 143, 12715–12724` and
`J. Am. Chem. Soc. 2024, 146, 3125–3135`) — both match this CSL exactly,
which is good validation that the translation below is correct.

**Correction from an earlier draft of this file:** article titles are in
**Title Case** (major words capitalized), not sentence case as previously
stated here — confirmed by the CSL's `text-case="title"` on the title
macro, and visible in the real examples below ("Nature of the N-H···S
Hydrogen Bond" — *Nature*, *Hydrogen*, *Bond* capitalized; *of*, *the*
lowercase).

## In-text citation placement

From the CSL `<citation>` block: numbers only (`citation-number`),
**superscript** (`vertical-align="sup"`), multiple citations at one point
joined by **comma with no space**, sorted by citation number, and
consecutive runs **collapse into en-dash ranges** (`collapse=
"citation-number"`).

- No brackets, no parentheses, no space before the number.
- A number attaches to the specific word/clause it supports, which may be
  mid-sentence — not necessarily batched at the sentence's end.
- Multiple citations: `4,5` (comma, no space).
- Three or more consecutive numbers collapse to a range: `6–11` (not
  `6,7,8,9,10,11`).

Real examples (from the source papers):
> "...plays a crucial role in its function and dysfunction.¹,²"
> "...sequence-based design,⁴,⁵ structure-based design,⁶⁻¹¹ and
> high-throughput screening (HTS),¹²⁻¹⁷ have been employed..."

## Reference list — general shape

Every entry: `(N)` + author list + type-specific body + DOI/URL if
available. References are numbered **in first-citation order**, not
alphabetically, and that number is fixed for that source throughout the
paper. Page ranges are **expanded**, not abbreviated (`page-range-format=
"expanded"` — write `12715–12724`, not `12715–24`).

**Authors** (all types): `Last, F. M.; Last, F. M.; Last, F. M.` — every
author initialized and inverted to Last-first (not just the first author),
semicolon-separated, **no "and"** before the last name, no "et al."
truncation built into the style itself (a very long author list may still
use "et al." by the target journal's separate policy — see the Gaussian
example below, which does).

## Reference types, with formats and examples

### Journal article (`article-journal`, `review`)
```
(N)  Last, F. M.; Last, F. M. Title of the Article in Title Case.
     Abbrev. Journal Name Year, Volume (Issue), StartPage–EndPage.
```
- Title: Title Case, not italic, ends with a period.
- Journal name: **abbreviated** form, italicized.
- Year: **bold**.
- Volume: italicized. Issue number, if present, in parentheses right after
  volume (not italic) — often omitted for ACS journals paginated
  continuously by volume, as in both real examples below.
- Pages: en-dash range, no "pp." label.
- DOI appended at the end if available: `https://doi.org/...`

Real examples:
> (1) Biswal, H. S.; Wategaonkar, S. Nature of the N-H···S Hydrogen Bond.
> *J. Phys. Chem. A* **2009**, *113*, 12763−12773.

> (2) Chand, A.; Sahoo, D. K.; Rana, A.; Jena, S.; Biswal, H. S. The
> Prodigious Hydrogen Bonds with Sulfur and Selenium in Molecular
> Assemblies, Structural Biology, and Functional Materials. *Acc. Chem.
> Res.* **2020**, *53*, 1580−1592.

### Preprint / magazine or newspaper article (`article`, `article-magazine`, `article-newspaper`)
```
(N)  Last, F. M. Title of the Article in Title Case. Container Name
     (italic). Month Day, Year, pp StartPage–EndPage.
```
Use this for a ChemRxiv/bioRxiv/arXiv preprint: container-title is the
preprint server name (e.g., *ChemRxiv*), full month-day-year date (not just
year), and a "pp" page label if the preprint has assigned page/article
numbers. DOI appended if available (preprints usually have one).

### Book / report / other monograph-like source (`book`, `report`, etc.)
```
(N)  Last, F. M.; Last, F. M. Title of the Book in Title Case, Nth ed.;
     Editor, E. E., Ed.; Series Name; Publisher: City, Year; Vol. X,
     pp StartPage–EndPage.
```
- Title: **italic**, Title Case.
- Edition: ordinal + "ed." if numeric (e.g., "3rd ed."), else the edition
  field as given, both followed by a period.
- Editor (if the whole work is edited rather than authored): name(s) +
  ", Ed." / ", Eds."
- Publisher block: `Publisher: City`, then year.
- Volume/pages only if citing a specific volume or page range.
- A `report` type additionally inserts a genre + number (e.g.,
  "Tech. Rep. 123") before the publisher block.

Real example — validates this branch exactly, including the "Revision
A.03" edition field which isn't a bare number so it prints as given:
> (75) Frisch, M. J.; Trucks, G. W.; Schlegel, H. B.; Scuseria, G. E.;
> Robb, M. A.; Cheeseman, J. R.; Scalmani, G.; Barone, V.; Petersson, G.
> A.; Nakatsuji, H. et al. *Gaussian 16*, Revision A.03; Gaussian Inc.:
> Wallingford, CT, 2016.

### Thesis / dissertation (`thesis`)
```
(N)  Last, F. M. Title of the Thesis in Title Case. Genre (e.g., Ph.D.
     Dissertation), University Name, Year.
```
Title not italicized. "Publisher" here means the degree-granting
institution (no separate place field, per the CSL's thesis-specific
publisher macro).

Example (constructed from the CSL logic, format only — not a real cited
thesis):
> (N) Smith, J. A. Synthesis and Characterization of Novel Sulfur-Containing
> Fluorophores. Ph.D. Dissertation, National Taiwan University, 2022.

### Patent (`patent`)
```
(N)  Last, F. M. Title of the Invention in Title Case. Patent Number,
     Month Day, Year.
```
Title not italicized, followed by the patent number, then the full issue
date spelled out as text (not just the year).

Example (format only):
> (N) Doe, J. Q. Method for Preparing Sulfur-Substituted Chromenones. U.S.
> Patent 10,123,456, March 5, 2020.

### Book chapter / conference paper / encyclopedia entry (`chapter`, `paper-conference`, `entry-dictionary`, `entry-encyclopedia`)
```
(N)  Last, F. M. Chapter or Paper Title in Title Case. In Title of the
     Book or Proceedings (italic); Editor, E. E., Ed.; Series Name;
     Publisher: City, Year; Vol. X, pp StartPage–EndPage.
```
The chapter/paper title itself is not italicized; "In" precedes the
italicized container title (book or proceedings name) — except for
dictionary/encyclopedia entries, which omit "In" and go straight to the
italicized container title.

### Dataset / software / other unlisted type (fallback)
```
(N)  Last, F. M. Title. Container/Repository Name (italic), Year,
     Volume, Page/identifier.
```
This is the CSL's generic fallback branch, used for any source type not
explicitly covered above (e.g., a dataset or software citation). DOI/URL
appended if available.

### Website / blog post (`webpage`, `post`, `post-weblog`)
```
(N)  Last, F. M. Title of the Page (italic). Site or Organization Name.
     URL (accessed Year-Month-Day).
```
Title is italicized here specifically (unlike every other type's title
macro). Because webpages usually lack a DOI, the URL + accessed-date form
is used instead (the CSL's `access` macro falls back to URL+date for any
type other than article-journal/book/chapter/encyclopedia/dictionary/
paper-conference when no DOI is present).

## DOI / URL rule (applies to every type)

If the source has a DOI, append `https://doi.org/<DOI>` at the end of the
entry, no matter the type. Only if there's no DOI *and* the type isn't one
of journal-article/book/chapter/encyclopedia-entry/dictionary-entry/
conference-paper does the entry fall back to `URL (accessed
YYYY-MM-DD)`.
