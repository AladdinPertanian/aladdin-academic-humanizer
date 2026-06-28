<!--
Copyright (c) 2026 Dr. Aladdin Ali - Founder of Aladdin Pertanian Internasional - dr.alaa@aladdin.my.id. All Rights Reserved.
-->

# Worked Examples (English v1)
## Skill reference — P4 build
### Each example shows the three channels, preserves every number/citation/DOI, and the consent gate

> These are illustrative. **Every example preserves numbers, citations, and DOIs byte-for-byte** (INV-A1),
> applies thought-level changes **only in Channel 3 on consent** (INV-A5/A6), and produces a **revision log**
> for any Channel-3 run (INV-A10). Example 2 demonstrates the **consent gate**: with consent withheld,
> Channel 3 is not produced.

---

## Example 1 — Overclaim + de-AI, full pipeline (consent granted)

**Contract:** `level=journal` · `programme_type=journal` (originality expected) · `edit_scope=apply_approved_notes`
· `co_authored=false` · `ai_disclosure_policy=required` · `output_language=en`.

**Input (author's Discussion paragraph):**
> "In conclusion, our groundbreaking study leverages a robust new method that clearly proves Drug X causes
> bleeding. Studies show this is a pivotal finding. In our trial, 20 of 25 patients experienced bleeding
> (see Table 2), consistent with Almeida et al. [7]."

### Channel 1 — Language-Improved Text (auto, expression-only)
> "Our study uses a new method that clearly proves Drug X causes bleeding. Studies show this is an important
> finding. In our trial, **20 of 25** patients experienced bleeding (see **Table 2**), consistent with
> Almeida et al. **[7]**."

*Changed (expression only):* "In conclusion," removed (HUM-25); "groundbreaking" removed (HUM-01);
"leverages a robust" → "uses a" (HUM-07); "pivotal" → "important" (§B lexicon).
*Preserved:* the claim **and its booster** "**clearly proves … causes**" — removing "clearly" would change
claim strength, so it **stays in Channel 1** and the over-claim is handled in Channel 2 (ACA-01); the uncited
"Studies show" (HUM-05 is advisory in academic mode); and **`20 of 25` · `Table 2` · `[7]`** — byte-for-byte
(INV-A1).

### Channel 2 — Scholarly Advisory Report (suggested, not applied)
- **A-01 (ACA-01 · overclaim/data-fidelity):** "proves that Drug X causes bleeding" exceeds a single
  20-of-25 trial. Suggested study-scoped, hedged rephrase: *"In this sample, bleeding was observed in 20 of
  25 patients, which **may indicate** a safety concern warranting further study."* *(claim-strength change —
  your call)*
- **A-02 (HUM-05 / ACA-02 · vague attribution):** "Studies show this is an important finding" is uncited —
  cite the specific studies, qualify, or remove.

### Author consent
`consent_to_apply = granted`, accepted: **A-01, A-02** (author chooses to *remove* the uncited sentence);
`authorship_acknowledgement = affirmed`.

### Channel 3 — Author-Approved Scholarly Revision (applied + humanised)
> "Our study uses a new method to examine the relationship between Drug X and bleeding. In our trial,
> **20 of 25** patients experienced bleeding (see **Table 2**), which **may indicate** a safety concern
> warranting further study, consistent with Almeida et al. **[7]**."

### Revision log (INV-A10)
**Header:** `en` · `journal`/`journal` · `apply_approved_notes` · `co_authored=false` ·
`ai_disclosure_policy=required` → Template A emitted · accepted: `A-01, A-02` ·
`authorship_acknowledgement=affirmed`.

| change_id | location | channel | approved_item_id | before → after | rationale | invariant_check |
|-----------|----------|:-------:|------------------|----------------|-----------|-----------------|
| C-001 | Discussion ¶ | Ch.3 | A-01 | "method that clearly proves Drug X causes bleeding … In our trial, 20 of 25 patients experienced bleeding → method to examine the relationship between Drug X and bleeding … In our trial, 20 of 25 patients experienced bleeding, which may indicate a safety concern warranting further study" | author accepted the study-scoped, hedged rephrase (causal over-claim removed) | INV-A6: claim narrowed by author choice; numbers untouched |
| C-002 | Discussion ¶ | Ch.3 | A-02 | "Studies show this is an important finding. → *(removed)*" | author accepted removal of the uncited attribution | INV-A2/A3: nothing fabricated; author's removal |
| C-003 | Discussion ¶ | Ch.1 | — (HUM-01/07/25) | "In conclusion, our groundbreaking study leverages a robust new method → Our study uses a new method" | expression-only de-AI | INV-A6: meaning preserved |

**Fidelity & attestation:** `20 of 25` → unchanged · `Table 2` → unchanged · `[7]` → unchanged. No scientific
limitation removed; no weak→strong change without an approved item. Disclosure: Template A included; no
"undetectable/detector-safe" claim. **Primary research responsibility remains with the author.**

---

## Example 2 — Consent gate (consent **withheld** → no Channel 3)

**Contract:** `level=masters` · `programme_type=masters_thesis` · `edit_scope=language_clarity` ·
`co_authored=false` · `ai_disclosure_policy=unknown` · `output_language=en`.

**Input:**
> "You can clearly see in Figure 3 that the model doesn't really work well, which underscores a pivotal
> limitation. The error rate was 12.4%."

### Channel 1 — Language-Improved Text (auto, expression-only)
> "Figure 3 shows that the model does not really perform well, which indicates an important limitation. The
> error rate was **12.4%**."

*Changed (expression only):* "You can clearly see in Figure 3" → "Figure 3 shows" (ACA-04 you→impersonal);
"doesn't really work well" → "does not really perform well" (contraction + "work"→"perform" register — the
downtoner **"really" is kept**; removing it would strengthen the claim → that is Channel 2); "underscores" →
"indicates" (§B); "pivotal" → "important" (§B). *Preserved:* the downtoner "really" and **`12.4%`**
byte-for-byte (INV-A1).

### Channel 2 — Scholarly Advisory Report (suggested, not applied)
- **B-01 (ACA-08 · descriptive→critical):** "does not really perform well" is evaluative but unquantified —
  consider stating the comparison/threshold that makes a **12.4%** error rate "not well".

### Author consent
`consent_to_apply = withheld`.

### Result — Channel 3 is **NOT produced**
Channels 1 and 2 are delivered in full. **Channel 3 is absent; no advisory item was applied; no revision
log was produced.** The `12.4%` error rate is unchanged. *(Disclosure: `ai_disclosure_policy=unknown` → an
advisory disclosure is still offered; silence is never an outcome.)*

> **Consent-gate proof:** thought-level item **B-01 was not applied**; the input's data is byte-for-byte
> intact; **Channel 3 was withheld** because its five conditions were **not** met (consent withheld) —
> exactly the gate behaviour (Blueprint §11 G1).

---

*Skill reference — P4 build. © 2026 Dr. Aladdin Ali / Aladdin Pertanian Internasional.*
