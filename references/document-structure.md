# ACS Journal Article — Document Structure

Derived from the observed section order in the three JACS articles supplied
as references (all published in *J. Am. Chem. Soc.*, so this reflects JACS
specifically — confirm against the target journal's own Instructions for
Authors if it's a different ACS journal, since section order/names vary
somewhat by journal and article type).

## Observed section order

1. **Title** — descriptive, states the finding/system, not a question.
2. **Author list** — full names, affiliation superscripts, corresponding
   author(s) marked with `*`.
3. **Abstract** — one paragraph, no citations, no subheadings. Often paired
   with a **TOC/abstract graphic** (a small summary figure).
4. **Introduction** — no "Introduction" content before it (starts right
   after the abstract/graphic); ends by stating what the paper reports,
   often the same novelty sentence echoed from the abstract.
5. **Results and Discussion** — combined section (not split into separate
   "Results" then "Discussion" sections) in all three source papers.
   Subheadings break it into named stages, e.g.:
   - "Synthesis and Characterization"
   - "Steady-State Photophysical Properties"
   - "Time-Resolved Photophysical Properties"
   - "Computational Approach"
   Each subheading is a bolded run-in or a small caps header, not a new
   top-level numbered section.
6. **Conclusion** — short, no new data; restates the main finding and its
   significance, often with one forward-looking sentence ("further
   research is currently in progress" / similar).
7. **Associated Content** — standard ACS block:
   - **Supporting Information** — one paragraph pointing to the SI PDF via
     DOI link, then a bullet/run-in list of exactly what the SI contains
     (e.g., "Discussions of experimental procedures, synthetic methods,
     photophysical properties, ... (PDF)").
   - **Accession Codes** — e.g., CCDC numbers for crystal structures, with
     how to retrieve them.
8. **Author Information**
   - **Corresponding Author(s)** — name, affiliation, email, ORCID.
   - **Author(s)** — remaining authors, affiliations, ORCID where given.
   - **Author Contributions** — who contributed equally, etc.
   - **Notes** — competing-interest / conflict-of-interest statement.
9. **Acknowledgments** — funding sources, grant numbers, named
   colleagues/facilities.
10. **References** — numbered in citation order (see
    `citation-format.md`).

## Figure/scheme/table numbering (cross-reference)

Per `style-guide.md` Chapters 15–17: figures, tables, and
charts/schemes are **separate numbering sequences**. In the source papers:
- `Figure 1`, `Figure 2`, ... for spectra, structures, plots.
- `Scheme 1`, `Scheme 2`, ... for synthetic routes.
- `Table 1`, `Table 2`, ... for tabulated data (e.g., photophysical
  parameters).
- Compound numbers (boldface, e.g., **3NTF**, **10**) are their own
  identifier system, assigned once and reused consistently in prose,
  schemes, and any tables — not renumbered per section.

## Still needed to complete this file

This is based on JACS specifically. If the target journal is different
(e.g., *Org. Lett.*, *Anal. Chem.*, *ACS Nano*, *Chem. Mater.*), its
Instructions for Authors page may specify a different section order, word
limits, or additional required sections (e.g., a separate "Experimental
Section" instead of folding methods into Results and Discussion, or a
required "Author Contributions" via CRediT taxonomy). Paste that journal's
guidelines and this file will be split by journal if needed (see the
`SKILL.md` domain-organization note).
