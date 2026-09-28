# ACS Tone Examples

Excerpts from three published papers supplied by the user, chosen from the
Abstract, Introduction, and Results/Discussion sections — the parts of a
paper that carry the most tone/voice (Methods and SI are more mechanical).
Each excerpt is annotated with the rhetorical pattern it demonstrates, so
the skill can reproduce the *pattern*, not just quote these sentences.

Sources:
1. Wang, Liu, Huang, Chen, Meng, Liao, Liu, Chang, Li, Chou. *J. Am. Chem.
   Soc.* **2021**, *143*, 12715–12724. ("3NTF" thiol-ESIPT paper)
2. Wang, Wang, Wu, Chang, Wang, Liu, Chen, Chou. *J. Am. Chem. Soc.*
   **2024**, *146*, 3125–3135. ("NTFs" follow-up paper)
3. Springer, Zanon, Taghavi, Sung, Disney. *J. Am. Chem. Soc.* **2025**,
   *147*, 34271–34282. (RNA-reactive covalent binders paper)

## 1. Broad-to-narrow opening ("textbook fact, then the twist")

> "Along the group 16 (VIA) family of the periodic table, the conventional
> wisdom learned from textbooks tells us that only H₂O possesses a hydrogen
> bond that explains its abnormally high boiling point that cannot fit into
> the correlation of increasing boiling point with increasing molecular
> weight from H₂S and H₂Se to H₂Te. However, this does not rule out the
> existence of H-bonds for other group 16 family members." (Source 1,
> Introduction, opening lines)

**Pattern:** start from an established, almost textbook-level fact the
reader already accepts, then pivot on "However" to the specific gap the
paper addresses. This is the default ACS Introduction opening move — don't
open with "In this paper" or a generic topic sentence; open with the field's
settled assumption and complicate it.

## 2. Anticipating and naming reader skepticism

> "One may be skeptical about why reports on the photophysics of thiol
> H-bonded molecules are so scarce. Chemically, one major reason lies in
> its instability... It requires special caution to exclude air during the
> synthesis and purification to prevent the occurrence of oxidation."
> (Source 1, transition into Results and Discussion)

**Pattern:** explicitly voice the doubt a critical reader would have
("why is this understudied?") and answer it with a concrete mechanistic or
practical reason, rather than ignoring the question. This is a
mechanism-forward, argumentative move — it treats the reader as an active
skeptic to be persuaded, not a passive recipient of facts.

## 3. Gap statement via "however" contrast (Abstract-level)

> "RNA is a key drug target that can be modulated by small molecules;
> however, covalent binders of RNA remain largely unexplored." (Source 3,
> Abstract, first two sentences)

**Pattern:** the classic two-clause abstract opening — clause 1 establishes
why the topic matters (independently verifiable, not argued), clause 2
pivots on "however" to the specific unsolved problem the paper tackles. Very
compressed; no throat-clearing.

## 4. Citation-dense scene-setting sentence

> "RNA structure, both in noncoding (nc) and coding transcripts, plays a
> crucial role in its function and dysfunction.¹,² Thus, one way to
> modulate RNA function is by targeting its structure³ such as
> sequence-based design,⁴,⁵ structure-based design,⁶⁻¹¹ and
> high-throughput screening (HTS),¹²⁻¹⁷ have been employed to identify and
> optimize small molecules for RNA targeting." (Source 3, Introduction,
> opening paragraph)

**Pattern:** a single sentence can legitimately carry 3–4 distinct citation
points, each attached to the specific sub-claim it supports (see
`citation-format.md` for the exact superscript mechanics). This density is
normal in an ACS Introduction's literature-survey paragraphs — it is not
overcitation, because each number is doing real work, not decorating a
generic claim.

## 5. Explicit statement of novelty, hedged but direct

> "We report here, for the first time, the experimental observation on the
> excited-state intramolecular proton transfer (ESIPT) reaction of the
> intrinsic thiol proton in room-temperature solution." (Source 1, Abstract,
> opening sentence)

**Pattern:** ACS abstracts state the novelty claim plainly and early
("for the first time," "we report here") rather than burying it. This is
confident but scoped precisely to what was actually shown — not "we
revolutionize" but "we report the experimental observation of X."

## 6. Mechanism-forward causal chaining in Results/Discussion

> "The electron-donating diethylamino group at the 4′-position elongates
> the π-conjugation by coupling with the carbonyl electron acceptor (see
> Figure 1) and hence retaining most of the dominating ππ* character in the
> S₁′ geometry (Figure 7) and hence the remarkable 710 nm tautomer
> emission." (Source 1, Conclusion)

**Pattern:** results are narrated as a causal chain (`substituent X` →
`elongates conjugation` → `retains ππ* character` → `produces the observed
emission`), each link tied to a specific figure/table, not left as isolated
observations. "Hence," "thus," "consequently," and "as a result" are the
connective tissue between data and interpretation — prefer them over
listing observations as a flat sequence.

## 7. Integrated figure/scheme references inside argument, not just captions

> "As shown in Figure 3a, we start from N-NTF in cyclohexane, where N-NTF
> reveals a major absorption band that is maximized at 380 nm. Upon
> excitation at the absorption peak wavelength, the emission is dominated
> by a 695 nm emission band. By monitoring at the 695 nm emission band, the
> corresponding excitation spectrum maximized at 380 nm is identical to the
> absorption spectrum (Figure 3a). Therefore, the 695 nm emission with a
> Stokes shift as large as ∼12,000 cm⁻¹... is reasonably assigned to the
> proton-transfer tautomer emission via the −SH-associated ESIPT, as
> previously concluded for 3NTF." (Source 2, Results)

**Pattern:** figures are cited inline as evidence *within* a sentence that
is making a claim ("As shown in Figure 3a, ..."; "(Figure 3a)" mid-sentence
as a parenthetical), not only referenced once and then discussed in the
abstract. "Therefore," "reasonably assigned to" signal that the conclusion
is being derived from the cited data in front of the reader, step by step.

## 8. Precise, calibrated hedging — not vague qualifiers

> "This viewpoint can also be further supported by the mid-IR spectra of
> 3TFs, where a broad and weak S−H stretching mode absorption can be
> observed at 2493, 2502, and 2500 cm⁻¹ for 3NTF (see Figure 2), 3TF, and
> 3FTF, respectively." (Source 1, Results)

**Pattern:** claims are hedged with specific epistemic verbs tied to the
evidence type — "supported by," "consistent with," "reasonably assigned
to," "indicates," "suggests" — each calibrated to how strong the evidence
actually is (X-ray/NMR data → stronger verbs like "confirm"/"demonstrate";
computational estimates → softer verbs like "suggest"/"estimated to be").
Avoid both overclaiming ("proves") and empty hedging ("might possibly
perhaps").

## Quick tone checklist derived from these examples

1. Does the Introduction open with an established fact before pivoting to
   the gap, rather than starting with "In this study..."?
2. Does the Abstract state the novelty claim plainly in the first 1–2
   sentences ("we report," "for the first time"), scoped to what was
   actually shown?
3. Is every citation attached to the specific sub-claim it supports (per
   `citation-format.md`), rather than batched at a paragraph's end?
4. Are results narrated as a causal chain ("X leads to Y, and hence Z"),
   with each link pointing at a specific figure/table?
5. Is every figure/table cited inline, mid-argument, not just listed once?
6. Does each hedging verb ("suggests," "confirms," "is consistent with")
   match the actual strength of the evidence behind it?
