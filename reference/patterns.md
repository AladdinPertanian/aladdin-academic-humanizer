<!--
Copyright (c) 2026 Dr. Aladdin Ali - Founder of Aladdin Pertanian Internasional - dr.alaa@aladdin.my.id. All Rights Reserved.
-->

# Pattern taxonomy — HUM-01..33 (reused) + ACA-01..10 (academic-integrity) — 43 patterns

© 2026 Dr. Aladdin Ali / Aladdin Pertanian Internasional. All rights reserved.
HUM-01..30 are the humanizer base sections §1–30 (open-source "humanizer" skill by Siqi Chen —
github.com/blader/humanizer, v2.8.0, MIT, (c) 2025), whose taxonomy traces to Wikipedia's "Signs of AI
writing" (CC BY-SA 4.0). **HUM-31..33 are Siqi Chen's own additions in the humanizer project (MIT) — they
are NOT drawn from the Wikipedia article** (manufactured punchlines, aphorism formulas, conversational
rhetorical openers). ACA-01..10 and all academic-integrity governance are original proprietary work.
See [../NOTICE](../NOTICE) *(present in P1; its third-party attribution aligns with this Skill's `NOTICE`,
which mirrors the agricultural NOTICE's MIT base attribution and the CC BY-SA upstream credit, kept
legal-open)*.

> **CC BY-SA — legal-open (academic skill).** Whether the academic patterns are uncopyrightable
> *ideas* (no share-alike) or *adapted material* (share-alike applies) is a legal question, **not
> asserted here as fact**. No verbatim Wikipedia text is reproduced; every pattern wording and
> before→after example here is the humanizer project's (MIT) or the Owner's own. The Wikipedia-derived
> base taxonomy (`HUM-01..30`) is kept **clearly marked**, while `HUM-31..33` (Siqi Chen's own MIT
> additions) and the Owner's original `ACA-01..10` are kept **separable**, pending legal confirmation
> before release (Blueprint v3 §7).

Each pattern: **id · source · severity · channel · what it is · before → after**, where *source* is
the humanizer base section (`§N`) or `Wikipedia survey`, and *channel* is where it acts:
**Channel 1** = automatic, expression-only (Language-Improved Text) · **Channel 2** = advisory,
surfaced not applied (Scholarly Advisory Report) · **Channel 3** = applied only on explicit author
consent (Author-Approved Scholarly Revision).
Severity order for application: **critical → high → medium → low**. Never alter a number, unit, date,
quoted span, citation, or DOI (INV-A1). v1 = English; non-English channels arrive in P5.

---

## A. De-AI core — HUM-01..33 (Channel 1, expression-only)

The de-AI patterns clean formulaic, generic, or low-quality phrasing on **writing-quality grounds** —
clarity, register, convention — **never** to reduce a "detector score" (no such concept exists here,
INV-A8). They are
**Channel 1 (AUTO)** unless noted. Each preserves meaning, data, and citations.

### Critical

- **HUM-01 · §1 · Ch.1 · Significance inflation** — drop hype adjectives.
  `groundbreaking → significant`, `revolutionary → new`, `unprecedented → unusual`, `paradigm-shifting → notable`.
  - Before: "This groundbreaking study fundamentally transforms our understanding of the field."
  - After: "This study contributes new evidence to the field."

- **HUM-04 · §4 · Ch.1 · Promotional language** — remove marketing tone ("rich literature", "cutting-edge", "state-of-the-art" as praise).
  - Before: "This cutting-edge framework offers a powerful, elegant solution."
  - After: "This framework offers a solution to the stated problem."

- **HUM-05 · §5 · Ch.2 (advisory — NOT Channel 1; academic reclassification) · Vague / unsupported attributions** — In academic mode this is **advisory only**. Removing an attribution wrapper ("studies show", "research suggests", "it is widely believed") **changes the evidential framing** of the claim — it makes an unsupported claim read as the author's direct judgement — so it is **never auto-applied in Channel 1**. Channel 1 **leaves the text unchanged**; Channel 2 **flags** the vague/unsupported attribution and the author decides whether to cite the specific source, qualify, or rephrase. *(Like HUM-24's ACA-07 constraint, this reclassifies a parent Channel-1 pattern, because in academic writing the attribution frame is evidentially meaningful.)*
  - Channel 1: text left unchanged.
  - Channel 2 (advisory, not applied): "'Studies show that this method is superior' uses a vague, uncited attribution — cite the specific studies, qualify the claim, or rephrase (ACA-01 / ACA-02)."

- **HUM-07 · §7 · Ch.1 · AI vocabulary overuse** — `leverage → use`, `utilize → use`, `delve into → examine`, `facilitate → help`, `robust → strong/reliable`, `crucial/pivotal → important`. See the **academic lexicon** (Section B) for the academic extension.

- **HUM-08 · §8 · Ch.1 · Copula avoidance** — "serves as a / acts as a / stands as a" → "is a".
  - Before: "The sample size serves as a key limitation of the study."
  - After: "The sample size is a key limitation of the study."

- **HUM-11 · §11 · Ch.1 · Synonym cycling** — stop renaming the same referent each sentence ("the participants" → "the subjects" → "the cohort"); pick one canonical term and keep it. *(Cross-ref ACA-06; choosing the canonical term among genuine variants is the author's — Channel 2.)*

- **HUM-14 · §14 · Ch.1 · Em/en-dashes** — replace `—`/`–` used as connectors with a comma or period; for numeric ranges convert `20–30` to `20 to 30`, **never dropping a number** (INV-A1).

- **HUM-18 · §18 · Ch.1 · Emojis** — remove all emojis (academic register: none).

- **HUM-20 · §20 · Ch.1 · Chatbot artefacts** — delete "As an AI", "I hope this helps", "Feel free to ask", "Let me know if you need anything", "I'd be happy to".

- **HUM-22 · §22 · Ch.1 · Sycophantic / servile tone** — delete "Certainly!", "Great question!", "Absolutely!".
  - Before: "Great question! Certainly, the results are discussed below."
  - After: "The results are discussed below."

- **HUM-24 · §24 · Ch.1 (CONSTRAINED by ACA-07) · Excessive hedging** — thin **contentless stacked filler** ("it might perhaps possibly be the case that") to a single honest qualifier. **Never remove a modal/epistemic hedge ("may", "suggests", "is consistent with") that carries claim strength** — that is a Channel-2 suggestion applied only in Channel 3 on consent.
  - Before: "It could perhaps possibly be argued that the effect may be present."
  - After: "The effect may be present." *(keeps the one epistemic hedge "may")*

- **HUM-25 · §25 · Ch.1 · Generic positive conclusions** — cut "In conclusion, this important work opens exciting new avenues" filler endings; keep a substantive, scoped conclusion the author wrote.

- **HUM-28 · §28 · Ch.1 · Signposting / announcements** — delete "Let's dive in", "In this section we will explore", "It is worth noting that" when contentless.

### High

- **HUM-03 · §3 · Ch.1 · Superficial -ing analyses** — "highlighting the importance of…", "showcasing…", "underscoring…" tacked onto a clause → cut or make a plain clause. *(If it masks missing analysis, also flag ACA-08 in Channel 2.)*
- **HUM-10 · §10 · Ch.1 · Rule of three** — break forced triads ("novel, robust, and impactful") when padding; keep only the true items.
- **HUM-12 · §12 · Ch.1 · False ranges** — "anywhere from a few to several" → a real number or "varies". Never fabricate a figure (flag in Channel 2 if data is absent).
- **HUM-21 · §21 · Ch.1 · Knowledge-cutoff disclaimers** — delete "as of my last update", "I don't have real-time data".
- **HUM-23 · §23 · Ch.1 · Filler phrases** — "it is important to note that", "needless to say", "at the end of the day" → remove.
- **HUM-27 · §27 · Ch.1 · Persuasive authority tropes** — "the gold standard", "widely regarded as" → remove unless sourced (else flag ACA-02).
- **HUM-33 · §33 (Siqi Chen, MIT) · Ch.1 · Conversational rhetorical openers** — "Ever wondered why…?", "Here's the thing:" → cut.

### Medium

- **HUM-02 · §2 · Ch.1 · Notability name-dropping** — gratuitous famous names → remove (keep genuine, cited attributions).
- **HUM-06 · §6 · Ch.1 · Formulaic challenges** — "While X, it is important to Y" filler frame → state the substance.
- **HUM-09 · §9 · Ch.1 · Negative parallelisms** — "It's not just X, it's Y" → state Y.
- **HUM-13 · §13 · Ch.1 · Passive / subjectless fragments** — give the action a subject where clarity improves (academic passive for methods is legitimate — do not over-correct; see ACA-04/ACA-05).
- **HUM-15 · §15 · Ch.1 · Boldface overuse** — strip bold used for emphasis spam.
- **HUM-16 · §16 · Ch.1 · Inline-header vertical lists** — "**Method:** … **Result:** …" mid-paragraph → prose or a real list.
- **HUM-19 · §19 · Ch.1 · Curly quotes** — `“ ” ‘ ’` → straight `" '` (unless the venue style requires typographic quotes — `venue_policy`).
- **HUM-26 · §26 · Ch.1 · Hyphenated word-pair overuse** — "high-impact, well-designed, data-driven" pile-ups → thin out.
- **HUM-30 · §30 · Ch.1 · Diff-anchored writing** — "Unlike the previous draft…" meta-commentary → remove.
- **HUM-31 · §31 (Siqi Chen, MIT) · Ch.1 · Manufactured punchlines / staccato** — "And that changes everything." one-line drama → remove.
- **HUM-32 · §32 (Siqi Chen, MIT) · Ch.1 · Aphorism formulas** — "When it comes to research, less is more." → remove.

### Low

- **HUM-17 · §17 · Ch.1 · Title case in headings** — sentence case (unless `venue_policy` requires title case).
- **HUM-29 · §29 · Ch.1 · Fragmented headers** — merge orphaned one-word headers.

---

## B. Academic formulaic-phrase lexicon (extends HUM-07, Channel 1)

An academic extension of the AI-vocabulary set — formulaic / generic phrasing over-represented in
low-quality academic prose. Replace on **writing-quality grounds** (precision, not tell-counting),
**preserving meaning**. These are suggestions toward plain-precise-formal register, not blanket bans —
keep a word when it is the precise term.

| Over-used token | Plainer / more precise |
|-----------------|------------------------|
| delve into | examine, study, analyse |
| underscore / underscores | show, emphasise, indicate |
| testament to | evidence of, shows |
| pivotal / crucial | important, central, key |
| intricate / multifaceted | complex, detailed |
| nuanced (as filler) | qualified, specific |
| realm / landscape / arena (figurative) | field, area, literature |
| tapestry / interplay (decorative) | interaction, relationship |
| shed light on | clarify, explain, show |
| navigate (the challenges) | address, manage, handle |
| foster / cultivate (figurative) | support, develop, promote |
| paramount / vital | essential, important |
| holistic (vague) | comprehensive, whole-system *(only if accurate)* |
| leverage / harness | use, apply |
| in the realm of | in |
| a myriad of | many, numerous |

**Constraint:** this lexicon is **Channel 1** and never changes a claim. If replacing a word would
alter claim strength or meaning (e.g. "may" vs "does"), it becomes a Channel-2 suggestion (ACA-07).

---

## C. Academic-integrity patterns — ACA-01..10 (channel-tagged, source-tagged)

Owner-proprietary. These replace the agricultural-safety patterns (AGR-01..05) with
academic-integrity controls. Channel tag governs how each acts; **every pattern is source-tagged**.

**Sources legend.** `[Q]` Qassim University thesis guide · `[T]` Tørresen master-thesis guide ·
`[ART]` Ecarnot et al. scientific-article guide · `[THE]` Burns scientific-style thesis (tag definitions in
[integrity.md](integrity.md) §3 and [../NOTICE](../NOTICE)). **These are source *tags***; the full
verifiable manifest (URLs · access dates · checksums) is in [sources.md](sources.md) (Blueprint §2.4).
Named sources — *GMU* (GMU Writing Center,
*Hedges*) · *Manchester* (Academic Phrasebank, *Cautious language*) · *APA* (APA Style, *Scholarly tone*) ·
*York* (Univ. of York, *Criticality*) · *EAP* (EAP Foundation, *Critical writing*) · *Wikipedia* ("Signs of
AI writing", CC BY-SA 4.0) — per Blueprint §2.2. These are point-in-time; re-verify before release
(Blueprint §9 #7).

- **ACA-01 · crit · Ch.2 → Ch.3 on consent · Overclaiming / data-fidelity · src [ART]·GMU** — flag a
  claim that exceeds its evidence; **suggest** a study-scoped, hedged rephrase (changing claim strength is
  the author's call). Apply only if accepted.
  - Before: "Drug X causes bleeding in patients."  *(from a single-trial Result)*
  - Advisory → After (on consent): "In this sample, bleeding was observed in most patients, which **may indicate** a safety concern warranting further study." *(Error = scope-inflation + causal implication; numbers untouched — INV-A1/A6.)*

- **ACA-02 · crit · Ch.1 preserve · Ch.2 flag · Citation integrity · src [Q][ART]·Wikipedia** —
  **preserve** every citation, reference, DOI, quoted span byte-for-byte (Channel 1); **flag** vague
  attribution, suspect, unresolvable, or unused references (Channel 2). **Never fabricate, complete, or
  "fix" a reference.**
  - Advisory: "Reference [12] is cited in the text but absent from the list — please verify."

- **ACA-03 · high · Ch.1 (AUTO) · Register elevation · src [Q][T]·APA** — colloquial/contraction/emotive
  → formal, meaning-preserving. Target = plain · precise · formal · **not** ornate.
  - Before: "We didn't really get why the model kind of fell apart here."
  - After: "It is not yet clear why the model's performance degraded in this case."

- **ACA-04 · high · Ch.1 (mechanical) · Ch.2/Ch.3 (restructure) · Person & voice · src [T]** — second
  person "you" → impersonal recast (auto, meaning-safe); first-person/"we" reduction that needs
  restructuring → advisory; `co_authored` governs whether "we" is retained.
  - Before: "You can see in Figure 2 that you get a higher yield."
  - After: "Figure 2 shows a higher yield."

- **ACA-05 · med · Ch.1 (mechanical) · Tense conventions · src [ART][THE]** — present for established
  facts/the system under study; past for methods, results, and others' specific findings. *(Apply only
  where unambiguous; otherwise advise — Channel 2.)*

- **ACA-06 · high · Ch.2 → Ch.3 on consent · Terminology consistency · src [T][THE]** — flag
  synonym-drift for one referent and missing acronym expansion at first use; **picking the canonical term
  is the author's**.
  - Advisory: "'participants', 'subjects', and 'cohort' refer to the same group — choose one."

- **ACA-07 · high · Ch.1 remove filler · Ch.2 suggest · Ch.3 apply on consent · Hedging (two-sided) · src GMU·Manchester**
  — **remove** contentless AI-hedge filler (Channel 1, carries no claim); **suggest** a calibrated
  hedge for an unqualified categorical claim (Channel 2 — adding a hedge changes claim strength).
  *Constrains HUM-24: never strip an epistemic hedge that carries claim strength.*
  - Advisory: "'This proves the hypothesis' overstates a single result — consider 'This is consistent with the hypothesis'."

- **ACA-08 · med · Ch.2 → Ch.3 on consent · Descriptive→critical signal · src York·EAP** — flag
  descriptive-only passages where criticality is expected, and "-ing decoration" pseudo-analysis. The
  critical thinking is the author's to supply; the tool only signals the gap.
  - Advisory: "This paragraph summarises the source but does not evaluate it — consider adding your critical assessment."

- **ACA-09 · med · Ch.2 → Ch.3 on consent · Structure / abstract / figure validation · src [Q][T][ART][THE]**
  — section presence/order; abstract length per `venue_policy`; figures/tables cross-referenced and
  discussed. **Only if `document_scope=full_document`**; on a bare fragment, mark *not-applicable*.
  - Advisory: "Figure 3 is not referenced in the text" / "No Limitations subsection found."

- **ACA-10 · med · Ch.2 → Ch.3 on consent · Title / abstract conventions · src [ART][THE]** — title as a
  precise label (keywords, no undefined abbreviations); abstract structured, stand-alone, introduces no new
  information. Numeric limits come from `venue_policy`, not a universal rule.

**ACA-01 vs ACA-07:** ACA-01 owns *flagging the over-claim*; ACA-07-add owns *suggesting the hedge
wording* — both advisory, both applied only in Channel 3 on consent.
**Data-fidelity rule:** no ACA pattern may remove an important scientific limitation or convert weak
evidence into a strong claim without explicit, logged author approval (INV-A6).

---

## D. Channel map — every pattern, at a glance (INV-A5/A6/A10)

| Channel | Patterns | Rule |
|---------|----------|------|
| **Channel 1 — auto, expression-only** | HUM-01..04, 06..33 *(HUM-05 excluded, see below)* · ACA-03 · ACA-04 (mechanical part) · ACA-05 · ACA-07 (filler-removal part) | meaning/data/claims unchanged (INV-A6); never touches thought-level (INV-A5). |
| **Channel 2 — advisory, surfaced not applied** | HUM-05 · ACA-01 · ACA-02 (flag part) · ACA-04 (restructure part) · ACA-06 · ACA-07 (hedge-suggestion part) · ACA-08 · ACA-09 · ACA-10 | the author decides; nothing thought-level is auto-applied (INV-A5). |
| **Channel 3 — applied only on explicit consent + revision log** | any Channel-2 item the author accepted | logged per [revision-log-spec.md](revision-log-spec.md) (INV-A10); claim-strength/limitation changes only here (INV-A6). |

*HUM-05 is reclassified to Channel 2 in academic mode (attribution framing is evidentially meaningful).
HUM-24's hedge removal is constrained by ACA-07. No pattern in any channel performs AI-tell measurement
(INV-A8).*

---

*Pattern taxonomy — P2 build (ACA source-tagged + channel map; full manifest at P4). Attribution mirrors `NOTICE`. © 2026 Dr. Aladdin Ali / Aladdin Pertanian Internasional.*
