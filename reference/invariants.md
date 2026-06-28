<!--
Copyright (c) 2026 Dr. Aladdin Ali - Founder of Aladdin Pertanian Internasional - dr.alaa@aladdin.my.id. All Rights Reserved.
-->

# Invariants & the Three-Channel Contract
## Skill reference — migrated from the P0 governance draft at P1 (canonical copy)
### Position Statement: formal channels · revision log · Channel-3 conditions

> **Canonical.** This is the **canonical** invariants reference for the Skill. The P0 review copy at
> `docs/academic-humanizer/p0-governance-drafts/invariants.md` is frozen history; edit **this** file.
> **Governing documents.** The owner *Position Statement* (this Skill's `README.md`, authored at P4) +
> Blueprint v3. Vocabulary: `INV-A` / *Channel 1/2/3* only (DEV-08).
> **Relationship.** [integrity.md](integrity.md) defines `INV-A*` as principles; this file restates them as
> an operational checklist and binds them to the three-channel contract, the Channel-3 conditions, and the
> revision log.

---

## 1. The three-channel contract (Position Statement §4)

| Channel | Name | Release | Function |
|:-------:|------|---------|----------|
| **1** | **Language-Improved Text** | automatic | **Editorial, not intellectual.** Expression-only edits (de-AI `HUM-*` + AUTO register). Numbers, %, units, dates, quoted spans, citations, DOIs preserved **byte-for-byte** (INV-A1). No meaning/claim change (INV-A6). |
| **2** | **Scholarly Advisory Report** | automatic — **suggested, not applied** | A professional academic review: overstatement/under-support · over-descriptive sections · weak results→discussion transitions · unclear methodology · questionable/incomplete references · figure/table interpretation gaps · possible AI-use disclosure need. The author decides. |
| **3** | **Author-Approved Scholarly Revision** | **only when the §3 conditions are met** | Applies **only** the Channel-2 items the author **explicitly accepted**, professionally + humanised, with a **revision log**. An editorial/revision service, **not** an authorship service. **The core purpose.** |

Channels are never silently merged: Channel 2 is never auto-folded into Channel 1; Channel 3 exists only
under explicit author consent (§3).

---

## 2. Pre-output invariant checklist (INV-A1..A10)

Each must hold before the relevant channel is emitted. A failed item blocks the **offending edit**, not the
whole run (the author still receives the legitimate channels).

| # | Invariant | Check | On failure |
|---|-----------|-------|------------|
| **INV-A1** | Byte-for-byte data fidelity | every number, %, unit, date, quoted span, citation, DOI in any channel is identical to the input. A datum/citation/DOI changes **only** on a **documented author correction** (corrected value **+ its source**, logged) — **consent alone is insufficient** (AIP-2/A3); else the original stands. | revert; the datum is untouchable. |
| **INV-A2** | No tool-originated scholarship | the tool never invents a claim, argument, finding, or conclusion of its own; in Channel 3 it **executes the author's approved decisions**. | remove it; it is the author's to write. |
| **INV-A3** | No fabrication | no citation, reference, statistic, result, or quote was invented or completed. | remove; flag the gap in Channel 2. |
| **INV-A4** | Honest about detection | no channel/label implies "undetectable" / "detector-safe" / "beats detectors"; no detector score used. | strip the phrasing (see §4). |
| **INV-A5** | Thought-level = consent-gated, never auto | nothing touching criticality, structure, claim-strength, or critical stance is applied in Channel 1; it is surfaced in Channel 2 and applied in Channel 3 **only on explicit approval** (logged). | move to Channel 2; apply only on approval. |
| **INV-A6** | Claim/limitation fidelity (extended per Position Statement §4) | Channel 1 never changes meaning, claim, or hedging strength of a sourced claim; **no channel may remove an important scientific limitation, or convert weak evidence into a strong claim, without explicit author approval recorded in the revision log.** | revert, or move to Channel 2 as a suggestion. |
| **INV-A7** | Same language in/out | `output_language` == input language; nothing translated. | block (v1 = `en`). |
| **INV-A8** | No detector-surrogate / no detectability objective | no count, score, threshold, before/after tell-count, or detector comparison — internal or external. | remove the measurement; patterns stand on quality merit (§4). |
| **INV-A9** | Develop, don't fabricate-from-nothing | work stayed within `edit_scope` (develop/refine/apply-approved); no whole content/data invented from nothing. | refuse the *fabricating* part only — never the legitimate help. |
| **INV-A10** | Channel 3 is auditable | every Channel-3 run produces a **revision log** recording each substantive change and the author-approved advisory item that justifies it (Position Statement §4). | no log → no Channel 3. |

**Reframe note.** INV-A5/A6/A9 do not *forbid* thought-level change outright — they **permit it through the
author's explicit, logged consent** (Channel 3). The integrity mechanism is **consent + auditability**, not
a block.

---

## 3. Required conditions for Channel 3 (Position Statement §4)

Channel 3 runs **only** when **all five** exist:

1. an original, author-provided text;
2. a Channel 1 (Language-Improved Text) version;
3. a Channel 2 (Scholarly Advisory Report);
4. **explicit author approval** of the advisory items to be applied (`consent_to_apply` + the accepted item IDs), carrying the author's `authorship_acknowledgement` (affirmed);
5. a **revision log** documenting what was changed and why (INV-A10).

Missing any one → Channel 3 is not produced; Channels 1 and 2 are still delivered in full.

**Acceptance test (consent gate).** With approval withheld → Channels 1 + 2 delivered, Channel 3 absent, no
thought-level advisory item applied, no revision log fabricated.

---

## 4. No measurement, of any kind (INV-A8) — quality, not policing

No aggregate AI-tell assessment: no counting, scoring, thresholding, before/after tell-count, or detector
comparison — internal or external — and no "reduce-detectability" objective. The tool has **no concept of
detectability** (Blueprint §5.8). Each `HUM-*` / `ACA-*` pattern is applied (Channel 1/3) or advised
(Channel 2) **solely on its own writing-quality merit**. The reason is fairness + quality (detectors are
biased against non-native writers), **not** suspicion of the author. The only forbidden marketing claim is a
false "undetectable / detector-safe" promise (a transparency requirement, INV-A4).

---

## 5. Accountability — the system supports, it does not certify (Position Statement §5)

The system does **not** determine whether a thesis or article is academically valid. **Primary research
responsibility remains with the author**; the **supervising professor, examiner, committee, journal editor,
or peer-review body** hold approval/acceptance authority. The system's responsibility is narrower: avoid
fabrication · preserve data/citation integrity · support required disclosure · document the AI-assisted
revision (the log) · avoid deceptive claims · keep authorship responsibility with the human author. **This
tool claims no research authorship or responsibility**, and **cannot verify** the truthfulness of an
authorship acknowledgement.

---

## 6. Tie to acceptance gates (Blueprint v3 §11)

| This file enforces | Gate |
|--------------------|------|
| Three-channel separation; INV-A5/A6 (Channel 1 meaning-safe; thought-level only on logged consent) | architectural |
| Channel-3 five conditions + revision log (INV-A10) | **G1** consent + audit gate |
| INV-A8 (no measurement) | **G4** No detector-surrogate |
| INV-A1 byte-for-byte data preservation | data-fidelity — **distinct from G2**, the *verifiable source manifest* in `reference/sources.md` (Blueprint §2.4) |
| Accountability / Human Authority Chain (§5) | **G6** — the tool supports (not enforces) integrity; claims no research responsibility |

Until the governance is signed off and the gates reconciled, the Skill stays **FOR REVIEW**.

---

*Skill reference (migrated from the P0 draft at P1) — © 2026 Dr. Aladdin Ali / Aladdin Pertanian Internasional.*
