<!--
Copyright (c) 2026 Dr. Aladdin Ali - Founder of Aladdin Pertanian Internasional - dr.alaa@aladdin.my.id. All Rights Reserved.
-->

# Integrity, Regulation & Authority Framework
## Skill reference — migrated from the P0 governance draft at P1 (canonical copy)
### Position Statement: responsible editing platform · supports (not enforces) · human authority

> **Canonical.** This is the **canonical** governance reference for the Skill. The P0 review copy at
> `docs/academic-humanizer/p0-governance-drafts/integrity.md` is frozen history; edit **this** file.
> **Governing documents.** The owner *Position Statement* (this Skill's `README.md`, authored at P4;
> source copy `docs/academic-humanizer/README.md`) + Blueprint v3 (`docs/BLUEPRINT-ACADEMIC-HUMANIZER-v3.md`).
> Attribution: [`../NOTICE`](../NOTICE).
> **Vocabulary.** Own vocabulary only — `AIP-*` (controls), `INV-A*`, *Input Contract*, *Channel 1/2/3*
> (DEV-08). Parent seams referenced by analogy only.

---

## 0. What this tool is — positioning (Position Statement §1)

The Academic Humanizer is a **responsible AI-assisted scholarly editing platform** that supports **lawful,
ethical, and academically supervised** improvement of research writing. It is **not** a restrictive
"integrity-enforcement gate", **not** an idea generator, **not** a citation/data inventor, and **not** a
detection-evasion tool.

There is **no** general academic or legal principle that treats using AI to review, polish, or improve an
*existing* scholarly text as inherently prohibited. The concern is **misuse** — undisclosed assistance
where disclosure is required, fabrication of sources/data, plagiarism, misrepresentation of authorship, or
breach of a university/journal/publisher policy. The platform is therefore governed by **responsible use,
transparency, human accountability, and institutional compliance** — **not** a presumption of prohibition.

---

## 1. Governance language — supports, does not enforce (Position Statement §3)

The correct governance statement is **not** "the system enforces academic integrity." It is:

> **The system supports responsible scholarly editing by structuring disclosure, preserving human
> accountability, preventing prohibited forms of fabrication or misrepresentation, and maintaining an
> auditable boundary between AI assistance and human authorship.**

Academic integrity **cannot be mechanically guaranteed by software**; it is an ethical and institutional
obligation held by the author, supervisor, and reviewing body. The system can **support** it, **document**
it (the Channel-3 revision log), and **refuse clearly improper uses (fabrication)** — but it **cannot
verify the truthfulness** of an authorship acknowledgement.

---

## 2. Human Authority Chain & accountability model (Position Statement §2, §5)

The thesis/article **text** is a **pre-final artifact**; the scholarly work — design, data, analysis,
supervision, defence, judgement — is larger than the document. The system does **not** decide whether a
thesis or article is academically valid. **Primary research responsibility remains with the
researcher/author**; the **supervising professor, examiner, committee, journal editor, or peer-review
body** hold supervisory, evaluative, and approval/acceptance authority (with their own institutional
responsibilities).

The system's responsibility is **narrower** — and that is the whole point:

- avoid fabrication;
- preserve data and citation integrity;
- support required disclosure;
- document the AI-assisted revision (the **revision log**);
- avoid deceptive claims;
- keep **authorship responsibility with the human author**.

**This tool claims no research authorship or responsibility.** Legitimate AI-assisted editing is conditioned
on: the author owning the intellectual content; no fabrication of data/citations/findings/conclusions;
disclosure where required; institutional/publisher policy respected; and the supervisor/examiner/journal/
committee retaining **final approval/acceptance authority** (Position Statement §2).

---

## 3. Academic Integrity Controls (AIP-1..6) — controls that *regulate*, not coerce

| ID | Control | What it regulates | Basis |
|----|---------|-------------------|-------|
| **AIP-1** | **Authorship & decision ownership** | The author owns the ideas, arguments, and editorial choices. The tool improves *expression* and, in Channel 3, **executes the author's approved decisions** — never inventing scholarship of its own. | Editors Canada · UNC |
| **AIP-2** | **Citation / data fidelity** | Preserve every citation, reference, DOI, number, and quoted span (Channel 1). *Flag* — never invent, complete, or silently alter — a suspect / unresolvable / unused reference. | [Q] [ART] [THE] · UNC |
| **AIP-3** | **No fabrication** | Zero invented data, statistics, sources, quotes, results. Missing → say so; never supply it. | all publisher bodies |
| **AIP-4** | **Transparency / disclosure-positive** | Offer (or, when required, produce) an AI-use disclosure. Never promise "undetectable / detector-safe"; never depend on a detector score. | COPE · ICMJE · Elsevier · Nature · Vanderbilt · Liang et al. |
| **AIP-5** | **EAL / ESL equity** | Language polish — especially for non-native writers — is fully legitimate; L1 directness is not a thought error. | T&F · Elsevier · Editors Canada |
| **AIP-6** | **No *silent* overstatement / limitation loss** | A change that shifts a claim beyond its evidence, **removes an important scientific limitation, or converts weak evidence into a strong claim** is surfaced (Channel 2) and applied only on logged author consent (Channel 3) — never auto-applied. | [ART] · GMU |

**Source tags.** `[Q]` Qassim · `[T]` Tørresen · `[ART]` Ecarnot et al. · `[THE]` Burns. Full manifest at
P4 (Blueprint §2.4 + Appendix B checksums). Policy sources + URLs: the Position Statement (README) §6 and
[`../NOTICE`](../NOTICE).

---

## 4. The three channels (operational shape — full spec in the Position Statement (README) §4)

| Channel | Name | Release | Role |
|:-------:|------|---------|------|
| **1** | **Language-Improved Text** | automatic | editorial-only; meaning/data/citations preserved (AIP-1/2/6, INV-A1/A6). |
| **2** | **Scholarly Advisory Report** | automatic — **suggested, not applied** | the author judges; nothing thought-level applied here (AIP-6, INV-A5). |
| **3** | **Author-Approved Scholarly Revision** | **only on the five conditions** ([input-contract.md](input-contract.md) §4 / [invariants.md](invariants.md) §3) | applies the author-accepted items + humanises + writes a **revision log**. The core purpose; an editing service, not authorship. |

Channel-3 conditions, the must-not list, and the revision log are specified in [input-contract.md](input-contract.md) §4 and
[invariants.md](invariants.md) §1–§3.

---

## 5. Disclosure-positive templates (AIP-4)

Driven by `ai_disclosure_policy` (`required` → include · `not_required` → offer · `unknown` → advise +
confirm venue). The author **adapts** these.

**Template A — language/clarity + author-approved revision:**
> *During the preparation of this work the author used an AI-based writing-development assistant (Aladdin
> Academic Humanizer) to improve the expression and readability of text the author had already written, and
> to apply revisions the author reviewed and explicitly approved. The assistant did not generate ideas,
> arguments, analysis, data, or citations. The author takes full responsibility for the content of the
> [manuscript / thesis / article].*

**Template B — advisory when `ai_disclosure_policy = unknown`:**
> *Advisory: confirm your venue's / institution's AI-use policy before submission. Most bodies (ICMJE,
> COPE, Elsevier, Nature, T&F, Wiley) require disclosing AI assistance and prohibit listing an AI tool as
> an author. Adapt Template A to the required wording.*

**Never produced:** any phrasing implying the text is "undetectable", "detector-safe", or "reads as 100%
human" (AIP-4 / INV-A4).

---

## 6. Responsibility boundary

The controls **regulate** honest use; they do **not** verify a person's honesty and never substitute for
human authority:

- the controls prevent fabrication and silent distortion; they do **not** block a legitimate author;
- the authorship acknowledgement is **lightweight and self-stated** — context + consent, not a proof of
  honesty; **the system cannot verify its truthfulness** (Position Statement §3);
- **primary research responsibility remains with the author** (§2); the supervisor and committee hold
  approval/acceptance authority. The tool **claims no research authorship or responsibility**.

Stating this boundary honestly is itself an AIP-4 (transparency) obligation.

---

## 7. Relationship to the acceptance gates (Blueprint v3 §11)

**G1** → a **consent + audit gate** (Channel 3 needs the five conditions incl. the revision log), not a
coercive attestation gate; **G3** (no unproven legal claims) and **G4** (no detector-surrogate) unchanged
and honoured; **G5** (originality from `programme_type`, not `level`) stays as a quality calibration;
**G6** asserts the Human Authority Chain (the tool supports, not enforces, integrity; claims no research
responsibility). **G2** (verifiable source manifest) is satisfied at P4 in `reference/sources.md`.

---

*Skill reference (migrated from the P0 draft at P1) — © 2026 Dr. Aladdin Ali / Aladdin Pertanian Internasional.*
