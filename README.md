<!--
Copyright (c) 2026 Dr. Aladdin Ali - Founder of Aladdin Pertanian Internasional - dr.alaa@aladdin.my.id.
All Rights Reserved.
-->

# Aladdin Academic Humanizer
## Academic Voice & Integrity Layer
### Responsible AI-assisted scholarly editing · Cloud Skill · `dependencies: none`

© 2026 Dr. Aladdin Ali / Aladdin Pertanian Internasional. All rights reserved.
See [LICENSE](LICENSE) and [NOTICE](NOTICE).

Aladdin Academic Humanizer is a responsible AI-assisted scholarly editing platform that improves
**existing** academic and research writing without replacing the author's intellectual work. It helps
students, researchers, and academics refine language, clarity, structure, scholarly tone, and presentation
while preserving the author's ideas, data, citations, quotations, numbers, and DOIs with strict fidelity.
It is part of the **Aladdin Agri AI** platform — <https://aladdin.my.id/smart-agricultural-advisor>.

> **In one line:** you bring text you already wrote; it returns (1) a cleaner version, (2) a professional
> review you decide on, and — only with your explicit approval — (3) a revised version with an audit log.
> It is **not** a ghostwriter, citation generator, plagiarism remover, or AI-detection evasion tool.

---

## Quick Start (for researchers)

**You provide:** academic text you have already written.
**You get back:** **Channel 1** (language-improved text) + **Channel 2** (a scholarly advisory report) —
and, *optionally*, **Channel 3** (an author-approved revision with a log) once you approve specific items.

**Three steps:**

1. **Ask for the review.** Open **[RESEARCHER-PROMPTS.md](RESEARCHER-PROMPTS.md)**, copy **Prompt A** in
   your language (10 languages provided), fill the bracketed fields, and paste your text.
   → returns **Channel 1 + Channel 2**.
   *If the Skill is already enabled, you can also just ask in plain language —* e.g. "Improve the language
   of this PhD chapter and give me an advisory report; discipline: agronomy; disclosure: required."

2. **Read Channel 2 and decide.** Each advisory note has an **ID**. Choose which IDs you accept; ignore the
   rest. If a note needs new data, a source, or evidence you did not supply, it is *flagged*, never invented.

3. **Apply, only if you want to.** Copy **Prompt B**, list the accepted item IDs, and confirm authorship.
   → returns **Channel 3 + a revision log**. Skip this step entirely if Channel 1 is all you need.

**After Channels 1–2, you are offered a next-step menu** — choose one: **(1)** keep the language correction
only; **(2)** proceed to a reviewed revision (you list the item IDs and confirm ownership of the text); or
**(3)** an expedited revision (confirm ownership; the tool auto-applies the safe, de-conflicted items). For
your protection, any change to a claim's strength, interpretation, data, numbers, or citations is **never**
auto-applied — it always needs your explicit yes.

> Same language in = same language out. Your **numbers, units, dates, quotations, citations, and DOIs are
> preserved exactly.** Nothing at the level of meaning, claims, or evidence changes without your approval.

### Which channel do I need?

| If you want to… | Use | Your approval needed? |
|---|---|:--:|
| Polish grammar, clarity, cohesion, and academic tone only | **Channel 1** | No |
| Get a professional critique (over-claiming, method, references, structure, disclosure) | **Channel 2** | No |
| Apply accepted critique items — humanised, with an auditable log | **Channel 3** | **Yes** (item IDs) |

### Set six quick fields (the Input Contract)

Tell the tool these six things once; they calibrate the output. Full rules:
[reference/input-contract.md](reference/input-contract.md).

| Field | Plain meaning | Choose from |
|---|---|---|
| `edit_scope` | What kind of editing | `language_clarity` · `register_elevation` · `copyedit` · `apply_approved_notes` (Channel 3) |
| `level` | How formal / critical the register should be | `undergraduate` · `masters` · `phd` · `journal` |
| `programme_type` | The originality expectation (set on its own — **never guessed from `level`**) | `undergraduate_assignment` · `masters_project` · `masters_thesis` · `research_masters` · `phd` · `journal` |
| `co_authored` | Controls the "we" vs. impersonal voice | `yes` · `no` |
| `ai_disclosure_policy` | Whether an AI-use declaration is added | `required` · `not_required` · `unknown` |
| `output_language` | Same as your text | one of the 10 supported languages |

*Optional but useful:* `discipline` (terminology + default citation style), `venue_policy` (journal/university
rules, word limit, abstract), `document_scope` (`full_document` enables structure/abstract/figure checks, or
`fragment`).

### Common scenarios (ready settings)

| Scenario | `edit_scope` | `level` | `programme_type` | Tip |
|---|---|---|---|---|
| Undergraduate essay polish | `language_clarity` | `undergraduate` | `undergraduate_assignment` | — |
| Master's thesis chapter | `register_elevation` | `masters` | `masters_thesis` | set `document_scope=full_document` for structure notes |
| PhD chapter + critique | `language_clarity` | `phd` | `phd` | read Channel 2 before any Channel 3 |
| Journal manuscript | `register_elevation` | `journal` | `journal` | paste the journal's AI policy into `venue_policy` |
| Conference paper | `register_elevation` | `journal` | `journal` | — |
| Abstract tightening | `copyedit` | *(your level)* | *(your type)* | set `document_scope=fragment` |

---

## What it is — and is not

It is an **editor and reviser, not an author.** It never originates an idea, argument, analysis, finding,
conclusion, statistic, source, or citation. It **supports** responsible scholarly editing (disclosure where
required, human accountability, no fabrication, and an auditable boundary between AI assistance and human
authorship); it **does not "enforce integrity"** and is **never** a detection-evasion tool.

**Use it** to polish the language/register/clarity of an assignment, thesis chapter, or manuscript; to get a
scholarly advisory review; or to produce an author-approved, humanised revision of accepted suggestions with
a revision log.

**Do not use it** to *generate* content (a literature review, a discussion, an abstract from results, a
conclusion, or citations from nothing), to translate between languages, or to make text "undetectable".

---

## Three-Channel Output Model

| Channel | Output | Function | Boundary |
|---------|--------|----------|----------|
| **Channel 1** | **Language-Improved Text** | Automatic editorial improvement of the author's existing text. | Preserves every number, unit, date, quoted span, citation, and DOI byte-for-byte. No meaning, claim, finding, or evidentiary-strength change. |
| **Channel 2** | **Scholarly Advisory Report** | Professional academic review: over-/under-claiming, criticality, methodology, references, structure, figure/table interpretation, and disclosure issues. | Advisory only. Nothing thought-level is applied automatically; the author decides what to accept, reject, or discuss with a supervisor. |
| **Channel 3** | **Author-Approved Scholarly Revision** | Applies only the Channel-2 items explicitly accepted by the author, professionally and humanely, with a revision log. | Not ghostwriting, not replacement authorship, and not an originality service. Every substantive change must be approved and logged. |

### Channel 1 — may improve / must not

**May improve:** clarity · grammar · readability · academic tone · cohesion · terminology consistency ·
sentence-level expression.
**Must not:** introduce new ideas · invent claims · alter findings · fabricate references · change data ·
change evidentiary strength without authorization.

### Channel 2 — may flag

Overstatement or under-supported claims · overly descriptive sections needing critical engagement · weak
transitions between results and discussion · missing or unclear methodological explanation · questionable,
incomplete, suspect, or unused references · figure or table interpretation gaps · possible need for AI-use
disclosure under institutional or journal policy.

### Channel 3 — may apply (with approval) / must not

**May apply, with approval:** accepted academic revisions · paragraph-structure improvements ·
section-coherence improvements · scholarly tone refinement · calibrated hedging where approved · clearer
relationships between findings and interpretation · improved presentation of existing arguments · preparation
for supervisor, committee, journal, or conference review.
**Must not:** add original analysis not present in the author's work · invent data, references, findings,
conclusions, or citations · materially change the thesis, argument, or interpretation without explicit
approval · remove important scientific limitations · convert weak evidence into strong claims · conceal AI
involvement where disclosure is required · market the output as "undetectable", "detector-safe", or
"100% human".

### Required conditions for Channel 3

Channel 3 runs only when **all five** conditions exist:

1. An original author-provided text.
2. A Channel 1 language-improved version.
3. A Channel 2 scholarly advisory report.
4. Explicit author approval of the advisory items to be applied (`consent_to_apply` + accepted item IDs).
5. A revision log documenting what was changed and why.

Formal rule: Channel 3 applies only those Channel-2 recommendations the author has explicitly accepted. The
output remains an editorial and academic-revision service, not an authorship service. Any change affecting
claim strength, interpretation, structure, or critical stance requires explicit author approval and remains
subject to supervisor, institutional, or journal review.

---

## Hard Boundaries

- Never originate an idea, argument, analysis, finding, conclusion, statistic, source, citation, or DOI.
- Preserve all numbers, units, dates, quoted spans, citations, and DOIs byte-for-byte unless the author
  supplies a documented correction with a source.
- Never fabricate missing content, references, results, or data.
- Never remove a scientific limitation or strengthen weak evidence without explicit, logged author approval.
- Never use, chase, report, or imply an AI-detector score.
- Never claim the output is "undetectable" or "detector-safe".
- Never translate; same language in, same language out.

---

## Language Coverage

The package is operative across all 10 supported languages:

`en` · `tr` · `ar` · `zh` · `id` · `es` · `fr` · `fa` · `ms` · `ur`.

English is shipped as v1. The remaining languages are source-grounded in
[reference/languages.md](reference/languages.md) and supported by per-language examples and per-language
prompts in [RESEARCHER-PROMPTS.md](RESEARCHER-PROMPTS.md). A final native-output review per language remains
the recommended last QA step.

---

## Governance & Professional Position

> Aladdin Academic Humanizer supports responsible scholarly editing by structuring disclosure, preserving
> human accountability, preventing prohibited forms of fabrication or misrepresentation, and maintaining an
> auditable boundary between AI assistance and human authorship.

**It is not an "integrity enforcement gate."** There is no general academic or legal principle that treats
using AI to review, polish, or improve an *existing* scholarly text as inherently prohibited. The legitimate
concern is misuse: undisclosed assistance where disclosure is required, fabricated sources or data,
plagiarism, misrepresentation of authorship, or violation of a university, journal, or publisher policy.
Accordingly, the Skill is governed by responsible use, transparency, human accountability, and institutional
compliance — not by a presumption of prohibition.

**Core academic principle.** A thesis, dissertation, manuscript, or research paper is the *textual
representation* of a broader scholarly process (research design, data collection, analysis, interpretation,
supervision, defence, revision, and final academic judgement). The written document is a critical
deliverable, but it is not the entire scholarly act. Using AI to improve the language, structure, clarity,
coherence, and presentation of an existing research text can be a legitimate part of scholarly development,
provided that: the author remains responsible for the intellectual content; no data, citations, evidence,
findings, or conclusions are fabricated; AI use is disclosed where required; institutional and publisher
policies are respected; and the supervisor, examiner, journal, or academic committee retains final authority.

**Accountability model.** Academic integrity cannot be mechanically guaranteed by software; it is an ethical
and institutional obligation held by the author, supervisor, and reviewing body. This Skill can *support*,
*document*, and *refuse clearly improper uses*, but it cannot verify the truthfulness of an authorship
acknowledgement. The system's responsibility is narrow: avoid fabrication; preserve data and citation
integrity; support required disclosure; document AI-assisted revision; avoid deceptive claims; and keep
authorship responsibility with the human author. **The Skill does not determine whether a thesis,
dissertation, or article is academically valid. Primary research responsibility remains with the author;
final supervisory, examination, editorial, or peer-review authority remains with the relevant human
institution.**

---

## Package Contents

| File | Purpose |
|------|---------|
| [SKILL.md](SKILL.md) | Frontmatter and fixed operating procedure: context + consent → Channel 1 → Channel 2 → Channel 3 on approval. |
| [RESEARCHER-PROMPTS.md](RESEARCHER-PROMPTS.md) | **Copy-ready researcher prompts in all 10 languages** — Prompt A (Channel 1 + 2) and Prompt B (Channel 3 authorization). Start here. |
| [reference/patterns.md](reference/patterns.md) | `HUM-01..33`, academic lexicon, `ACA-01..10`, channel tags, and channel map (43 patterns total). |
| [reference/integrity.md](reference/integrity.md) | AIP-1..6, INV-A1..A10, accountability model, no-detector-surrogate rule, and disclosure templates. |
| [reference/input-contract.md](reference/input-contract.md) | Contract fields and the Channel-3 five conditions. |
| [reference/invariants.md](reference/invariants.md) | Pre-output invariant checklist and three-channel contract. |
| [reference/revision-log-spec.md](reference/revision-log-spec.md) | Channel-3 revision-log format. |
| [reference/register.md](reference/register.md) | Register-elevation rules: plain, precise, formal, not ornate. |
| [reference/levels.md](reference/levels.md) | `level`, `programme_type`, and `co_authored` calibration. |
| [reference/languages.md](reference/languages.md) | 10-language framework, language constants, script-family handling, and Language-QA guidance. |
| [reference/sources.md](reference/sources.md) | Source manifest, checksums, URLs, access dates, and source notes. |
| [examples/before-after.md](examples/before-after.md) | English worked example with all three channels and a revision log. |
| `examples/before-after.*.md` | Per-language worked examples for the full supported language set. |
| [LICENSE](LICENSE) | Proprietary owner license with third-party carve-outs. |
| [NOTICE](NOTICE) | Copyright, trademarks, MIT attribution for the reused humanizer component, and CC BY-SA legal-open notice. |

---

## Policy Alignment

The governance model is aligned, as a point-in-time policy position, with major publication and editorial
guidance including ICMJE, COPE, Elsevier, and Nature Portfolio AI policies. Policies evolve; re-verification
before public release or institutional deployment is required. See
[reference/sources.md](reference/sources.md).

---

## Import and Packaging

The Skill is self-contained markdown and has `dependencies: none`. Package it as a single-root archive:

```text
aladdin-academic-humanizer/
  SKILL.md
  README.md
  RESEARCHER-PROMPTS.md
  LICENSE
  NOTICE
  reference/
  examples/
```

The archive must expose `SKILL.md` at the skill root after import. Use a packaging tool that writes
forward-slash paths inside the archive.

---

## Status

Current package status: **P1–P5**. English v1 is shipped; all 10 supported languages are grounded and
operative, with a final native-output review recommended per language. Version: `1.0.0-draft`.
