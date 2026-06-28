<!--
Copyright (c) 2026 Dr. Aladdin Ali - Founder of Aladdin Pertanian Internasional - dr.alaa@aladdin.my.id. All Rights Reserved.
-->

# Channel-3 Revision-Log Specification (INV-A10)
## Skill reference — P2 build
### The auditable boundary between AI assistance and human authorship

> **Why this exists.** Channel 3 (Author-Approved Scholarly Revision) **applies** advisory items the author
> accepted. INV-A10 makes that step **auditable**: every Channel-3 run **must** produce a revision log, and
> **no log → no Channel 3** ([invariants.md](invariants.md) §2–§3). The log is the documented,
> AI/author boundary the Position Statement §3–§5 requires; it is owner-proprietary governance.
> **Source-cited.** This format implements INV-A1/A5/A6/A10 and the Position Statement §4. It is **not**
> third-party material.

---

## 1. When a log is produced

A revision log is produced **only** on a Channel-3 run, i.e. when **all five** conditions hold
([input-contract.md](input-contract.md) §4): original text · Channel 1 produced · Channel 2 produced ·
`consent_to_apply = granted` + accepted item IDs (carrying `authorship_acknowledgement`) · this log. If any condition is missing, **Channel 3 and
its log are not produced** (Channels 1–2 still stand). A log is **never fabricated** to satisfy the gate.

---

## 2. Log structure

A Channel-3 revision log has three required parts: **(A) run header**, **(B) change ledger**, **(C)
fidelity & attestation**. Each Channel-3 change appears in the ledger and traces to an **accepted advisory
item ID** from Channel 2.

### A. Run header (contract summary)
| Field | Value |
|-------|-------|
| `output_language` | (e.g. `en`) |
| `level` / `programme_type` | (e.g. `masters` / `masters_thesis`) — `originality_requirement` derived |
| `edit_scope` | (e.g. `apply_approved_notes`) |
| `co_authored` | (bool — governs the "we" rule) |
| `ai_disclosure_policy` | `required` / `not_required` / `unknown` → which disclosure was emitted |
| `venue_policy` / `document_scope` | (if supplied) |
| `accepted_item_ids` | the Channel-2 item IDs the author approved (`consent_to_apply`) |
| `authorship_acknowledgement` | affirmed — recorded together with `consent_to_apply` as the Channel-3 consent |
| `timestamp` | ISO-8601, supplied by the runtime |

### B. Change ledger (one row per substantive change)
| `change_id` | `location` | `channel` | `approved_item_id` | `before → after` | `rationale` | `invariant_check` |
|-------------|------------|:---------:|--------------------|------------------|-------------|-------------------|
| C-001 | §3 ¶2 | Ch.3 | A-07 (ACA-07 hedge) | "proves the hypothesis → is consistent with the hypothesis" | author accepted the calibrated-hedge suggestion | INV-A6 (claim-strength change is author-approved) |
| C-002 | §2 ¶1 | Ch.1 | — (HUM-22 auto) | "Great question! The method… → The method…" | expression-only de-AI | INV-A6 (meaning unchanged) |

Rules for the ledger:
- **Every Channel-3 row MUST cite an `approved_item_id`** — a Channel-2 item the author accepted. A
  Channel-3 change with no approved item is forbidden (INV-A5).
- **Channel-1 (auto) edits** may be listed for completeness with `approved_item_id = —` and the pattern id
  (HUM-/ACA-); they are expression-only and never carry an approved-item requirement (INV-A6).
- **Claim-strength, limitation, structure, or critical-stance** changes appear **only** as Channel-3 rows
  with an `approved_item_id` (INV-A5/A6). None may appear as Channel-1.

### C. Fidelity & attestation
1. **Data-fidelity ledger (INV-A1).** List every number, %, unit, date, quoted span, citation, and DOI in
   the document and confirm it is **unchanged**. The only permitted change is a **documented author
   correction** — record the corrected value/citation **and its source**; **consent alone is never
   sufficient** (AIP-2/A3). Example row: `"n = 25" → unchanged`; `"[12] (1998)" → "[12] (1989)" — author
   correction, source: the cited paper's front matter`.
2. **No-unapproved-change attestation (INV-A5/A6).** Confirm: no thought-level change was applied without
   an `approved_item_id`; **no important scientific limitation was removed**; **no weak evidence was turned
   into a strong claim** without an approved item.
3. **Disclosure record (AIP-4).** State which AI-use disclosure was emitted (per `ai_disclosure_policy`) and
   that no "undetectable / detector-safe" claim was made (INV-A4).
4. **Authority note.** Restate that **primary research responsibility remains with the author** and the
   tool claims no research authorship/responsibility (Position Statement §5).

---

## 3. Worked micro-example

> **Header:** `en` · `masters`/`masters_thesis` (originality expected) · `apply_approved_notes` ·
> `co_authored=false` · `ai_disclosure_policy=required` → Template A emitted · accepted: `A-01`, `A-07`.
>
> **Ledger:**
> | C-001 | Discussion ¶1 | Ch.3 | A-01 (ACA-01 overclaim) | "Drug X causes bleeding in patients → In this sample, bleeding was observed in most patients, which may indicate a safety concern warranting further study" | author accepted the study-scoped rephrase | INV-A6: claim narrowed, numbers untouched |
> | C-002 | Discussion ¶1 | Ch.3 | A-07 (ACA-07 hedge) | "always → may" | author accepted the calibrated hedge | INV-A6: hedge added by author choice |
> | C-003 | Intro ¶2 | Ch.1 | — (HUM-07) | "leverage → use" | expression-only | INV-A6: meaning unchanged |
>
> **Fidelity:** "20 of 25 patients" → unchanged; "[7]", "10.1000/abcd" → unchanged. No limitation removed;
> no weak→strong change without an approved item. Disclosure: Template A included. Author holds research
> responsibility.

---

## 4. Invariants this spec enforces

- **INV-A10** — a log is produced for every Channel-3 run, or Channel 3 is withheld.
- **INV-A5** — every thought-level change traces to an accepted Channel-2 item.
- **INV-A6** — claim-strength / limitation changes are author-approved and logged; Channel-1 stays
  meaning-safe.
- **INV-A1** — the data-fidelity ledger **records and attests** that every datum/citation/DOI is unchanged
  (or a documented, sourced author correction).
- **AIP-4 / INV-A4** — the disclosure record is present; no detection-evasion claim.

---

*Skill reference — P2 build. © 2026 Dr. Aladdin Ali / Aladdin Pertanian Internasional.*
