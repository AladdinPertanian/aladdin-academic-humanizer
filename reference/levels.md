<!--
Copyright (c) 2026 Dr. Aladdin Ali - Founder of Aladdin Pertanian Internasional - dr.alaa@aladdin.my.id. All Rights Reserved.
-->

# Level, Programme-Type & Person Calibration
## Skill reference — P3 build
### `level` sets *register/criticality* · `programme_type` sets *originality* · `co_authored` sets *person*

> **Two separate fields.** `level` and `programme_type` are **independent** Input-Contract fields.
> **Originality is NEVER inferred from `level` alone** (gate **G5**; Blueprint §1.2) — a Master's
> *thesis/research* track is **expected by default** to make an original contribution (overridable by
> `venue_policy`/institution), while a Master's *taught/project* track may not.
> **Source-tagged** (`[Q][T][ART][THE]` + York/EAP — see [patterns.md](patterns.md) §C legend; full
> manifest at P4). These calibrate *expectations the advisory surfaces* — they never license the tool to
> add scholarship (INV-A2) or change a claim (INV-A6).

---

## 1. `level` — register & criticality tier (src [Q][T][ART][THE])

`level` tunes **how much** criticality, structure, and citation rigor the **Channel-2 advisory** expects.
Register elevation itself ([register.md](register.md)) targets the same *plain-precise-formal* at every tier.

| `level` | Audience | Criticality target | Structure model | Citation rigor |
|---------|----------|--------------------|-----------------|----------------|
| `undergraduate` | university students | competence | essay / report | format consistency |
| `masters` | Master's students | high | thesis | + gap framing |
| `phd` | PhD students | high | thesis | + comprehensive engagement |
| `journal` | research writing | high + external scrutiny | strict IMRaD + venue rules | + original-source + verify-each |

The tier raises the **bar the advisory flags against** (e.g. at `phd`/`journal`, ACA-08 expects critical
engagement, ACA-09 expects full structure). It does **not** change what Channel 1 does.

---

## 2. `programme_type` — originality expectation (src [Q][T][THE]·[ART]; gate G5)

`originality_requirement` is derived from **`programme_type`**, with `venue_policy`/institution as an
override — **never from `level` alone**.

| `programme_type` | `originality_requirement` (default) |
|------------------|-------------------------------------|
| `undergraduate_assignment` | not required |
| `masters_project` (taught / coursework) | not required |
| `masters_thesis` | **expected** (original contribution) |
| `research_masters` | **expected** |
| `phd` | **expected** |
| `journal` | **expected** |

**Override:** an explicit `venue_policy` or institutional rule supersedes the default.
**What the expectation does:** when originality is *expected*, the Channel-2 advisory may note where an
original contribution / critical stance is thin (ACA-08) or where a claim over-/under-reaches its evidence
(ACA-01). It **never** writes the contribution — that is the author's (INV-A2/AIP-1).

---

## 3. Acceptance test for G5 (operable)

| Input | Result |
|-------|--------|
| `level=masters` + `programme_type=masters_thesis` | originality **expected** |
| `level=masters` + `programme_type=masters_project` | originality **not required** |
| `level=masters` only (no `programme_type`) | **undetermined** — ask; never assume from `level` |

`level` alone never decides originality. (This is gate **G5**, [invariants.md](invariants.md) §6.)

---

## 4. Person rule — `co_authored` (src [T]; DEV-30/31)

Impersonal is the **default target**, **not a flat ban** — the first-person allowance follows
`venue_policy` and `co_authored`:

| Construct | Behaviour | Channel |
|-----------|-----------|:-------:|
| second person "you" | → impersonal recast (meaning-safe) | **1 (auto)** |
| first person "we" / "I" needing restructure | reduce **only** if it improves register **and** the venue prefers impersonal | **2 (advisory)** |
| "we" when `co_authored = true` | **kept** — "we" reduction is **skipped** | — |
| "we" when `co_authored = false` (single author) | may be flagged as a style note per venue | **2 (advisory)** |

Never invent or remove an agent that changes who did what (INV-A2). See [register.md](register.md) §2.

---

## 5. How the contract drives the run

| Field | Drives | Where |
|-------|--------|-------|
| `level` | criticality/structure/citation bar of the **advisory** (Channel 2) | §1 → ACA-08/09, [register.md](register.md) |
| `programme_type` (+`venue_policy`) | `originality_requirement` → advisory notes on contribution/claim reach | §2 → ACA-01/08 |
| `co_authored` (+`venue_policy`) | the person/"we" rule | §4 → ACA-04 |
| `venue_policy` | all venue-specific numbers (abstract length, citation style, word limits) | DEV-18; never a universal |

All of the above shape the **Channel-2 advisory** and the **register** target; none lets the tool originate
content (INV-A2), change a claim (INV-A6), or apply a thought-level change without consent (INV-A5).

---

*Skill reference — P3 build. © 2026 Dr. Aladdin Ali / Aladdin Pertanian Internasional.*
