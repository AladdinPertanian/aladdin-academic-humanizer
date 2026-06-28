<!--
Copyright (c) 2026 Dr. Aladdin Ali - Founder of Aladdin Pertanian Internasional - dr.alaa@aladdin.my.id. All Rights Reserved.
-->

# Register-Elevation Rules
## Skill reference — P3 build
### Target = plain · precise · formal · not ornate. Elevates **expression**, never **content** (INV-A6).

> **Scope.** These rules raise the *expression* of academic text to a credible scholarly register. They
> are **Channel-tagged**: the mechanical, meaning-safe parts run in **Channel 1 (auto)**; anything that
> would restructure thought or change a claim is **Channel 2 (advisory)** and applied only in Channel 3 on
> consent. They **never** change meaning, claim strength, data, or citations (INV-A1/A5/A6).
> **Source-tagged** (`[Q][T][ART][THE]` + APA/Manchester/GMU/York/EAP — see [patterns.md](patterns.md) §C
> legend; full manifest at P4). The word-level lexicon lives in [patterns.md](patterns.md) §B; the de-AI
> core in [patterns.md](patterns.md) §A.

---

## 1. The target register (ACA-03 · src [Q][T]·APA)

**plain · precise · formal · not ornate.** Avoid **both** poles:
- not **colloquial/casual** (contractions, slang, chatty asides, emotive intensifiers), **and**
- not **ornate/obscure** (decorative metaphor, inflated diction, long Latinate padding).

Formal-not-ornate means: the simplest precise wording that a scholarly reader expects. If a plainer word
is equally precise, prefer it (cross-ref the formulaic-phrase lexicon, [patterns.md](patterns.md) §B).

| Move | Channel | Example |
|------|:-------:|---------|
| contraction → full form | **1 (auto)** | "doesn't → does not" |
| colloquial/emotive → neutral formal | **1 (auto)** | "a huge problem → a substantial problem" |
| ornate/inflated → plain precise | **1 (auto)** | "utilise a plethora of → use many" |
| vague intensifier → removed or quantified | **1 (auto)** *(if no claim change)* | "very important → important" |

**Boundary:** if removing an intensifier would change claim strength (e.g. "significant" as a statistical
term), it is **not** auto — it is a Channel-2 note (ACA-07/ACA-01). INV-A6.

---

## 2. Impersonal voice & person (ACA-04 · src [T]; governed by `levels.md`)

- **Second person "you" → impersonal recast** — **Channel 1 (auto, meaning-safe).**
  "you can see in Figure 2 → Figure 2 shows".
- **First person "I"/"we"** — governed by `co_authored` and `venue_policy` (see [levels.md](levels.md) §4).
  Impersonal is the *default target*, **not a flat ban**. Reducing "we" where it needs **restructuring** is
  **Channel 2 (advisory)**, and is **skipped when `co_authored = true`**.
- Never invent an agent or change who did what (INV-A2). The academic passive for methods is legitimate —
  do **not** over-convert it to active (cross-ref HUM-13, applied conservatively).

---

## 3. Tense conventions (ACA-05 · src [ART][THE])

- **present** — established facts, accepted knowledge, the system/text under study ("the model uses…");
- **past** — what was done and found: methods, results, and **others' specific findings** ("Smith (2019)
  reported…").

Apply **Channel 1 (mechanical)** only where the choice is **unambiguous**; where the tense carries a
nuance (e.g. a still-true general finding), **leave it and note it in Channel 2** (INV-A5). Never change a
tense in a quoted span (INV-A1).

---

## 4. Terminology consistency (ACA-06 · src [T][THE]) — Channel 2 (advisory)

- one referent → **one canonical term** (stop synonym-cycling: "participants/subjects/cohort");
- expand each acronym at **first use**.

**Picking the canonical term is the author's** — so this is **advisory** (the tool flags the drift and the
unexpanded acronym; the author chooses). It is applied in Channel 3 only on consent.

---

## 5. Cohesion & flow (src [ART][THE]·APA)

- **Sentence-level connectors and given-new ordering** that don't move ideas → **Channel 1 (auto)** where
  meaning-safe (e.g. fixing a dangling connector, joining a fragment to its clause — cross-ref HUM-13).
- **Paragraph/section restructuring**, reordering arguments, or merging/splitting that changes emphasis →
  **Channel 2 (advisory)** — that is thought-level (INV-A5); never auto.
- Splitting an over-long sentence is allowed in Channel 1 **only at safe clause boundaries** and **never
  severing a number from its unit** (INV-A1).

---

## 6. What register elevation must NEVER do

- change meaning, claim strength, or hedging of a sourced claim (INV-A6) — that is Channel 2/3;
- make the text **ornate/obscure** (the failure opposite to colloquial);
- alter any number, unit, date, quoted span, citation, or DOI (INV-A1);
- remove a scientific limitation or upgrade weak evidence (INV-A6) — Channel 2/3 only, logged;
- "translate" register across languages (v1 = English; INV-A7);
- perform any AI-tell measurement (INV-A8).

---

## 7. Channel summary (mirror of [patterns.md](patterns.md) §D)

| Channel 1 (auto, expression-only) | Channel 2 (advisory) |
|-----------------------------------|----------------------|
| formality (§1), "you"→impersonal (§2), unambiguous tense (§3), sentence-level cohesion (§5) | "we"-restructure (§2), ambiguous tense (§3), terminology choice (§4), paragraph restructuring (§5) |

Calibration of *how much* criticality/structure to expect comes from `level`/`programme_type`
([levels.md](levels.md)); register elevation itself is the same target at every tier.

---

*Skill reference — P3 build. © 2026 Dr. Aladdin Ali / Aladdin Pertanian Internasional.*
