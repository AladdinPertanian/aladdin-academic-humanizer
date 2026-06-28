<!--
Copyright (c) 2026 Dr. Aladdin Ali - Founder of Aladdin Pertanian Internasional - dr.alaa@aladdin.my.id. All Rights Reserved.
-->

# Input Contract (context + consent)
## Skill reference — migrated from the P0 governance draft at P1 (canonical copy)
### Position Statement: context + consent · Channel-3 five conditions · revision log

> **Canonical.** This is the **canonical** Input-Contract reference for the Skill. The P0 review copy at
> `docs/academic-humanizer/p0-governance-drafts/input-contract.md` is frozen history; edit **this** file.
> **Governing documents.** The owner *Position Statement* (this Skill's `README.md`, authored at P4) +
> Blueprint v3. Vocabulary: `AIP` / `INV-A` / *Input Contract* / *Channel 1/2/3* only (DEV-08).

---

## 0. What the contract is for

The Input Contract is **context + consent**, not a coercive integrity gate (Position Statement §1, §3).
It does two honest jobs:

1. **Context** — the parameters needed to calibrate well (`level`, `programme_type`, `venue_policy`,
   `discipline`, language, document scope, disclosure policy).
2. **Consent** — the **lightweight authorship acknowledgement** and the **explicit author approval** that
   authorises **Channel 3**.

It **assumes legitimate use** — developing a research *text* with AI is **generally legitimate when
consistent with applicable institutional, publisher, and legal requirements** (Position Statement §1–§2) —
and **never withholds legitimate help to police the author**. The system **cannot verify** the truthfulness
of the acknowledgement (Position Statement §3); final approval/acceptance authority rests with the
**supervisor + examination committee** ([integrity.md](integrity.md) §2).

---

## 1. Contract fields

| Field | Required | Allowed values | Purpose |
|-------|:--------:|----------------|---------|
| `authorship_acknowledgement` | **– for Channels 1–2 · ✔ for Channel 3** | affirmed | A **contextual, non-blocking** acknowledgement that the text is the author's own. It does **not** gate Channels 1–2 (no confession required, §4); it is required **only** alongside `consent_to_apply` at Channel 3. Self-stated context, **not** a proof of honesty (the system cannot verify it). |
| `edit_scope` | ✔ | `language_clarity` · `register_elevation` · `copyedit` · `apply_approved_notes` | The kind of development requested. `apply_approved_notes` drives Channel 3 (§4). |
| `level` | ✔ | `undergraduate` · `masters` · `phd` · `journal` | Register / criticality only — not originality (§2). |
| `programme_type` | ✔ | `undergraduate_assignment` · `masters_project` · `masters_thesis` · `research_masters` · `phd` · `journal` | Originality calibration (§2; gate G5). |
| `co_authored` | ✔ | bool | Governs the first-person-plural ("we") rule. |
| `ai_disclosure_policy` | ✔ | `required` · `not_required` · `unknown` | Drives the AI-use disclosure (§3). Never inferred silently. |
| `output_language` | ✔ | `en` (v1) | Same language in/out (INV-A7); +9 languages in P5. |
| `consent_to_apply` | ✔ *for Channel 3* | granted / withheld **+ the accepted advisory item IDs** | The explicit author approval of which Channel-2 items to apply (§4). |
| `discipline` | – | STEM / humanities / … | Terminology + default citation style. |
| `venue_policy` | – | target style + word/abstract limits | All venue-specific numbers (never a universal law). |
| `document_scope` | – | `full_document` · `fragment` | Gates thesis-wide / figure checks; on a bare `fragment` those are *not-applicable*, never guessed. |

---

## 2. `originality_requirement` — a calibration, from `programme_type`, not `level` (gate G5)

A **calibration of expectations**, not a restriction. Never inferred from `level` alone: a Master's
*thesis/research* track expects an original contribution; a Master's *taught/project* track may not.

| `programme_type` | default |
|------------------|---------|
| `undergraduate_assignment` · `masters_project` | not required |
| `masters_thesis` · `research_masters` · `phd` · `journal` | **expected** |

`venue_policy` / institution **overrides** the default. **Test (G5):** `level=masters` + `masters_thesis` →
expected; + `masters_project` → not required.

---

## 3. Disclosure handling (AIP-4)

`required` → output **must** include a generated AI-use declaration (template in [integrity.md](integrity.md) §5);
`not_required` → **offered**; `unknown` → the tool **produces an advisory disclosure anyway** and asks the
author to confirm the venue policy. **Silence is never an outcome** — transparency is a positive default.

---

## 4. The Channel-3 consent gate — the only "gate", and it is consent + audit

Channels 1 (Language-Improved Text) and 2 (Scholarly Advisory Report) are offered as **ordinary legitimate
help** — no confession required. **Channel 3 (Author-Approved Scholarly Revision)** runs **only** when
**all five** Position-Statement conditions exist:

1. an **original, author-provided text**;
2. a produced **Channel 1**;
3. a produced **Channel 2**;
4. **explicit author approval** of the advisory items to apply (`consent_to_apply = granted` + accepted IDs), which **carries the author's `authorship_acknowledgement`** (affirmed) — the two together are the Channel-3 consent;
5. a **revision log** documenting each substantive change and its justifying, author-approved item.

Without all five, **Channel 3 is not produced** — Channels 1 and 2 are still delivered in full. This is the
inverse of the old coercive "no attestation → zero help" gate: **help is the default; consent + an audit
trail govern only the application of thought-level revisions, because that step enacts the author's own
editorial decisions** (Position Statement §4).

**`edit_scope` is scope-clarity + a fabrication boundary, not a refusal of help:** the tool develops,
refines, and applies the author's approved edits; it does **not** invent whole content, data, results, or
citations from nothing (AIP-3 / INV-A3) — a missing section or source is **flagged in Channel 2**, never
manufactured.

**Acceptance test (reframed G1 → consent + audit gate).** With `consent_to_apply` withheld → Channels 1+2
delivered, Channel 3 absent, no thought-level item applied, no revision log fabricated.

---

## 5. After consent — the procedure

> establish context + consent → de-AI core (`HUM-*`, expression-only) → **Channel 1** (Language-Improved
> Text) → **Channel 2** (Scholarly Advisory Report) → *(if the §4 five conditions are met)* apply the
> author-accepted items + humanise + write the revision log → **Channel 3** (Author-Approved Scholarly
> Revision).

The three-channel contract, the Channel-3 must-not list, and the per-channel invariants are in
[invariants.md](invariants.md); the accountability model is in [integrity.md](integrity.md) §1/§6.

---

*Skill reference (migrated from the P0 draft at P1) — © 2026 Dr. Aladdin Ali / Aladdin Pertanian Internasional.*
