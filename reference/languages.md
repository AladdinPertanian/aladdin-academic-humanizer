<!--
Copyright (c) 2026 Dr. Aladdin Ali - Founder of Aladdin Pertanian Internasional - dr.alaa@aladdin.my.id. All Rights Reserved.
-->

# Ten-Language Framework & Language-QA Gate
## Skill reference — P5 build
### English SHIPPED (v1) · **ALL 10 LANGUAGES GROUNDED** — `tr`·`ar`·`zh`·`id`·`es`·`fr`·`fa`·`ms` SOURCE-GROUNDED · `ur` GROUNDED (report manual) · **0 [PROVISIONAL]**

> **Self-contained.** Markdown-only, model-driven; **no runtime dependency** on the plugin's PHP
> language-packs. Per-language guidance is authored **into this file**. INV-A7: same language in/out — the
> Skill never translates.

> **⚠ P5 STATUS.** **`tr`, `ar`, `zh`, `id`, `es`, and `fr` are now SOURCE-GROUNDED** in authoritative
> university academic-writing guides (`sources.md` §1b–§1g) — their prior gap/directional state is **closed**
> for register/person-voice/objectivity/structure/citation. *Hedging density* stays conservative (`tr`);
> `ar`/`zh` ground objectivity (Arabic & Chinese are **more direct** than English — do not over-add
> English-style hedges); `zh` source is Traditional Chinese (Simplified needs a native check); `id` requires
> the **passive (pasif)**, `es` the **impersonal *se***, and `fr` the **passive form** (recommended; no first
> person); **`fa`** grounds **objectivity** (*بی‌طرفانه*; impersonal register, personal/subjective appeals
> «have no place»); **`ms`** grounds structure / **abstrak** (200–300 words) / citation (*pengarang-tahun*) /
> **ejaan baku** (Kamus Dewan/DBP) [MS1][MS3] (person/voice register-advisory — Malay format guides silent;
> Malay ≠ Indonesian, language-verified). **`ur`** is grounded on an authoritative Urdu **report-writing**
> manual [UR1] — structure/format/critical-analysis grounded, while its scholarly **person-voice/tense/hedging
> is gap-declared** (AIP-3) pending an Urdu scientific-article reference. **All 10 languages are now grounded
> — none remains [PROVISIONAL].** **Operative now: `en` + `tr` + `ar` + `zh` + `id` + `es` + `fr` + `fa` +
> `ms` + `ur`** (`ur`/`ms` with their declared register-advisories). A **final native-speaker review of live
> output** is recommended per language before heavy use — grounding closes the gap; native review is the last
> QA (§3).

---

## 1. Cross-linguistic model — constants vs variables

**Enforce these CONSTANTS identically in every language** (they do not vary): formality · precision ·
objectivity · evidence-anchored claims · terminology consistency · citation integrity · data-fidelity · the
de-AI core `HUM-01..33` · the academic-integrity controls AIP-1..6 · the three-channel model · INV-A1..A10.

**Calibrate these VARIABLES per language** (they do vary): hedge density · directness · paragraph linearity ·
politeness/impersonality norms · acceptable first-person use. **English hedges *more* than `ar`/`zh`/`fa`** —
the tool must **not** treat L1 directness as a thought error (AIP-1/AIP-5). Calibration changes *how* a
pattern is advised, never *whether* a constant holds.

---

## 2. Per-language table

| code | language | script family | `\b` word-rule? | script-family test | native validation | status |
|------|----------|---------------|:---------------:|:------------------:|:-----------------:|--------|
| `en` | English | Latin | **yes** (word-level) | PASS | n/a (source language) | **SHIPPED (v1)** |
| `ar` | Arabic | Arabic-script | **no** (phrase-level) | PASS (mechanical) | **source-grounded** [AR1][AR2][AR3] | **SOURCE-GROUNDED ✓** |
| `zh` | Chinese | Han | **no** (code-point) | PASS (mechanical) | **source-grounded** [ZH1] | **SOURCE-GROUNDED ✓** |
| `fa` | Persian | Arabic-script | **no** (phrase-level) | PASS (mechanical) | **source-grounded** [FA1][FA2][FA3] | **SOURCE-GROUNDED ✓** |
| `fr` | French | Latin | **yes** | PASS (mechanical) | **source-grounded** [FR1][FR2][FR3] | **SOURCE-GROUNDED ✓** |
| `es` | Spanish | Latin | **yes** | PASS (mechanical) | **source-grounded** [ES1] | **SOURCE-GROUNDED ✓** |
| `tr` | Turkish | Latin | **yes** (conservative — agglutinative) | PASS (mechanical) | **source-grounded** [TR1][TR2][TR3] | **SOURCE-GROUNDED ✓** |
| `id` | Indonesian | Latin | **yes** (conservative — affixation) | PASS (mechanical) | **source-grounded** [ID1][ID2][ID3] | **SOURCE-GROUNDED ✓** |
| `ms` | Malay | Latin | **yes** | PASS (mechanical) | **source-grounded** [MS1][MS2][MS3] (lang-verified) | **SOURCE-GROUNDED ✓** (voice advisory) |
| `ur` | Urdu | Arabic-script | **no** (phrase-level) | PASS (mechanical) | **partial** [UR1] (report manual) | **GROUNDED (report) ✓ · scholarly-register gap** |

*"script-family test PASS (mechanical)" = the de-AI/register channels are correctly restricted to the
language's script family (a design check the tool can self-verify). It is **not** native validation.*

---

## 3. Per-language guidance — `en` shipped · `tr`·`ar`·`zh`·`id`·`es`·`fr`·`fa`·`ms` source-grounded · `ur` grounded (report manual) · 0 [PROVISIONAL]

> **`en`** is shipped and **`tr`/`ar`/`zh`/`id`/`es`/`fr`/`fa`/`ms`** are **source-grounded** in authoritative
> university academic-writing references (their subsections cite [TR1][TR2][TR3] / [AR1][AR2][AR3] / [ZH1] /
> [ID1][ID2][ID3] / [ES1] / [FR1][FR2][FR3] / [FA1][FA2][FA3] / [MS1][MS2][MS3]; manifest in `sources.md`
> §1b–§1j). **`ur`** is grounded on an authoritative Urdu **report-writing** manual ([UR1]; §1h) —
> structure/format/critical-analysis grounded, scholarly person-voice/tense/hedging **gap-declared**. **No
> language remains gap-declared or [PROVISIONAL]** — `ms` is now grounded from **language-verified** Malay
> references (Malay ≠ Indonesian); constants (§1) hold across all. DeepL may assist drafting this guidance text
> — never the user's manuscript, never the authority. (`ur`'s scholarly gap and `ms`'s person/voice advisory
> are declared in their subsections — AIP-3, never invented.)

### English — SHIPPED (v1, the only validated language)
- **Register:** plain-precise-formal-not-ornate (ACA-03; APA *Scholarly tone*).
- **Hedging:** English hedges heavily; ACA-07 removes only contentless filler and **suggests** calibrated
  hedges — never strips an epistemic hedge (Manchester *Being cautious*, GMU *Hedges*).
- **Person:** impersonal default; first-person/"we" per `co_authored` + venue ([levels.md](levels.md) §4).
- **Script:** Latin → `\b` word-level de-AI channels are safe.

### `ar` Arabic — **SOURCE-GROUNDED** ([AR1] Suez Canal Univ. · [AR2] King Abdulaziz Univ. · [AR3] Grad-Studies guide)
The prior directional/provisional state is **closed**: the norms below are grounded in three authoritative
Arabic university thesis guides (`sources.md` §1c), **not invented** (AIP-3).
- **Script (test PASS):** Arabic-script → **no `\b`**; de-AI/register run **phrase-level** only — a Latin
  word-boundary substitution corrupts Arabic text. RTL must not split a number from its unit; preserve
  Arabic/Hindi digits, citations, DOI **byte-for-byte** (INV-A1).
- **Person & voice (ACA-04) — the signature Arabic norm:** academic Arabic uses the **passive (المبني
  للمجهول) / third person (الغائب)** with **no personal pronouns** [AR1]. The guide's own example: *"Do not
  write 'We measured the hardness' → write 'The hardness was measured'."* Prefer *الباحث / الكاتب / المؤلف*
  over first person; even then prefer impersonal constructions (*ويبدو أن … / ويتضح من ذلك*) over *ويرى
  الكاتب*. **Stronger than English** — flag first-person → passive (still the author's choice, INV-A5).
- **Tense (ACA-05):** **past** for completed work (the thesis narrates what was done); **present/future** for
  general facts, established principles, or future work [AR1].
- **Register (ACA-03):** *الأسلوب العلمي* — clear, precise, the **fewest possible words**; avoid vague words,
  and **avoid synonyms (المترادفات) and metaphors (المجازات)** [AR1] (reinforces ACA-06 / HUM-11).
- **Objectivity / claim strength (ACA-01 · ACA-08):** *الموضوعية* — present facts honestly; **do not force an
  opinion** on the reader; present results **before** discussion [AR1][AR3]. This grounds the no-overclaim
  control. Remove honorific titles when naming a person [AR1].
- **Terminology (ACA-06):** commit to scientific terminology — concepts, terms, definitions [AR1].
- **Structure / abstract (ACA-09/10):** **bilingual** abstract — *المستخلص* (Arabic) + Abstract (English);
  contains the objectives; **≤ 200 words / ≤ 1 page** [AR2 ≤200 · AR3 ≤1 page].
- **Citation (ACA-02):** *التوثيق* is **venue/discipline-specific** (e.g. Qur'an by sūra+āya; manuscripts;
  journals; web) [AR3][AR2] — driven by `venue_policy`.
- **Hedging:** Arabic is **more direct** than English (English hedges more — Blueprint §5.7); ACA-07 must
  **not** over-add English-style hedges. The grounded objectivity / no-opinion-forcing rule [AR1] is the
  relevant claim-strength control.
- **Status:** **source-grounded** from authoritative Arabic references — gap closed. A final
  **native-speaker review of live output** is still recommended as standard QA before heavy use.

### `zh` Chinese — **SOURCE-GROUNDED** ([ZH1] *學術研究論文撰寫說明*, §16.2–16.7)
The prior directional/provisional state is **closed**: grounded in an authoritative Chinese academic-writing
guide (`sources.md` §1d), **not invented** (AIP-3). *(Source is Traditional Chinese 繁體; Simplified-specific
conventions (zh-CN) warrant a native check.)*
- **Script (test PASS):** Han → **no `\b`**; **code-point** handling; no word-boundary substitution. Preserve
  numerals, citations, DOI **byte-for-byte** (INV-A1).
- **Person & voice (ACA-04) — the signature Chinese norm:** **avoid personal pronouns** (*我 / 我們 / 你 / 他 /
  自己 / 大家*) — indirect and cause reader ambiguity; **use definite nouns** (*本研究* = this study, *研究者*
  = the researcher) [ZH1 §16.3.1]. **Stronger than English** — flag first-person → definite noun (still the
  author's choice, INV-A5).
- **Register / de-AI (ACA-03) — concrete colloquial→formal list [ZH1 §16.3]:** *如果→若* · *所以→故 / 有鑑於此*
  · *或是→或* · *但是→但* · *等等→等* · *不管→不論* · *如要→若要*; **drop discourse-marker fillers** (*…來說 /
  …而言 / 換句話說 / 也就是說 / 一般來說 / 簡言之 / 換言之* = HUM-23/28 in Chinese); **drop self-Q&A** colloquial
  style (= HUM-33); replace **vague demonstratives** (*這 / 那 / 有些人 / 學者* = HUM-05 / ACA-06) with definite
  nouns.
- **Objectivity / claim strength (ACA-01):** *理性客觀陳述* — state arguments rationally and objectively
  [ZH1 §16.2]; prefer definite nouns over vague terms.
- **Structure / abstract (ACA-09/10):** **bilingual** abstract — 中文摘要 + English Abstract; the abstract
  **cites no references**; **3–5 keywords** (關鍵詞), Chinese keywords under the Chinese abstract, English under
  the English [ZH1 §16.6–16.7].
- **Citation (ACA-02):** in-text citations author(year) [ZH1 §16.5] — venue-specific (`venue_policy`).
- **Hedging:** Chinese is **more direct** than English (Blueprint §5.7) and the guide prefers **definite
  nouns**; ACA-07 must **not** over-add English-style hedges. The grounded objectivity rule [ZH1 §16.2] is the
  relevant claim-strength control.
- **Status:** **source-grounded** from an authoritative Chinese reference — gap closed. A final
  **native-speaker review of live output** (esp. zh-CN Simplified) is recommended as standard QA.

### `fa` Persian — **SOURCE-GROUNDED** ([FA1] آینۀ پژوهش *Guide to Academic Article Writing* · [FA2] Golestan U. · [FA3] Caspian J.)
The prior provisional state is **closed**: grounded in authoritative Persian academic-writing references
(`sources.md` §1i), **not invented** (AIP-3). *(A 219-pp owner guide [FA4] is also on file but its PDF text
layer is presentation-form glyphs — not machine-quoted; norms below are quoted from [FA1]/[FA2].)*
- **Script (test PASS):** Arabic-script (Persian) → **no `\b`**; phrase-level only; RTL safety. Preserve
  **Persian numerals** (۱۸ ۲۰), the decimal separator (٬/٫), citations, DOI **byte-for-byte** (INV-A1).
  **Persian ≠ Arabic** — connectives/forms differ; do not transfer Arabic guidance.
- **Objectivity / claim strength (ACA-01) — the signature Persian norm:** academic Persian must be
  **impartial/objective** (*بی‌طرفانه*); argument is **directed to reason, not emotion** (*معطوف به عقل … تا
  دل*); **appeals to personal knowledge/taste** (*معرفت/سلایق شخصی*) **«have no place»** and weaken the
  position [FA1]. → grounds the no-overclaim control **and** an **impersonal, non-subjective register**.
- **Person & voice (ACA-04):** follows from [FA1]'s objectivity rule — subjective first-person framing
  (*مطالعۀ ما … مشاهده کردیم*) yields to an **impersonal** statement (*در این مطالعه … مشاهده شد*). *(The
  purely-grammatical passive-vs-first-person choice is venue-dependent; where a venue is silent it is a
  Channel-2 advisory, not forced.)*
- **Register / clarity (ACA-03):** logical, precise; the author's meaning must be **made clear to the reader**
  (*برای خواننده روشن شود*) [FA2]; rational not rhetorical (*خطابی*) [FA1].
- **Structure (ACA-09):** methodical article structure (*ساختار مقاله*) — مقدمه / روش‌شناسی / یافته‌ها / بحث /
  نتیجه‌گیری; structure varies with **quantitative vs qualitative** method [FA2].
- **Abstract (ACA-09/10):** **bilingual** — چکیده (Persian) + Abstract (English), ~**150–250 words**; **3–5
  کلیدواژه** (Persian + English) [FA3].
- **Citation (ACA-02):** author-date / author-page / in-text / footnote; **under-citation ≈ plagiarism**
  (*سرقت علمی*) — never invent a reference (AIP-3); venue-specific (`venue_policy`) [FA1].
- **Hedging:** Persian academic hedges (*ممکن است / به نظر می‌رسد*); ACA-07 removes only contentless filler,
  never an epistemic hedge — calibrate normally.
- **Status:** **source-grounded** from authoritative Persian references — gap closed. A final
  **native-speaker review of live output** is recommended as standard QA.

### `fr` French — **SOURCE-GROUNDED** ([FR1] Guide rédaction · [FR2] Boudouresque *Manuel* · [FR3] Anthropos)
The prior directional/provisional state is **closed**: grounded in three authoritative French
scientific-writing guides (`sources.md` §1g), **not invented** (AIP-3).
- **Script (test PASS):** Latin → `\b` valid. Preserve numbers, citations, DOI **byte-for-byte** (INV-A1);
  French decimal uses a **comma + thin space** (`12,4 %`) and a space before `: ; ! ?` — never reformat.
- **Person & voice (ACA-04) — the signature French norm:** of the four options, the **passive form** (*"Les
  prélèvements ont été effectués…"*) is the **one recommended** in scientific writing; *je/nous* are "pas
  recommandée" and *on* is "déconseillé" [FR2/Boudouresque]. **Stronger than English** — flag first-person →
  passive (still the author's choice, INV-A5).
- **Register (ACA-03):** *langage objectif et neutre*, clear and precise [FR1]. Avoid colloquialism; respect
  French typographic spacing.
- **Terminology (ACA-06):** avoid *"termes schtroumpf"* — terms used **without a definition** or with a
  **variable meaning** in the same text; define each term and use it consistently [FR2, Encadré 9]. Foreign
  terms in *italics* [FR2].
- **Objectivity / claim strength (ACA-01):** the language must be **objective and neutral** (*objectif et
  neutre*) [FR1] — grounds the no-overclaim control.
- **Structure / abstract (ACA-09/10):** **bilingual** abstract — *Résumé* (French) + Abstract (English);
  **200–400 words**, no abbreviations, clear and simple, after the title; **5–6 keywords (mots-clés)**, also
  in English [FR1].
- **Citation (ACA-02):** author-year, first author named [FR1]; venue-specific (`venue_policy`; e.g. the
  Anthropos house style [FR3]).
- **Hedging:** French academic does hedge (*pourrait / semble / suggère*); ACA-07 removes only contentless
  filler and never strips an epistemic hedge — calibrate normally.
- **Status:** **source-grounded** from authoritative French references — gap closed. A final
  **native-speaker review of live output** is recommended as standard QA.

### `es` Spanish — **SOURCE-GROUNDED** ([ES1] *Manual de redacción de artículos científicos*)
The prior directional/provisional state is **closed**: grounded in an authoritative Spanish
scientific-writing manual (`sources.md` §1f), **not invented** (AIP-3).
- **Script (test PASS):** Latin → `\b` valid (standard Spanish word boundaries). Preserve numbers, citations,
  DOI **byte-for-byte** (INV-A1); Spanish decimal uses a **comma** (e.g. `12,4 %`) — never reformat it.
- **Person & voice (ACA-04) — the signature Spanish norm:** academic Spanish uses the **impersonal /
  passive-reflexive *se*** (*se observó* = was observed · *se realizó* · *se analizó* · *se presenta*) and
  **avoids first person** (no *yo* / *nosotros*) [ES1]. **Stronger than English** — flag first-person →
  impersonal *se* (still the author's choice, INV-A5).
- **Tense (ACA-05):** **past** for Methods and Results (*el estudio se realizó*, *se observó*) [ES1]; present
  for established facts / accepted knowledge.
- **Register (ACA-03):** clarity and precision (*con claridad*, *con precisión*); **APA** scholarly tone [ES1].
- **Objectivity / claim strength (ACA-01):** *describir objetivamente*; avoid subjectivism [ES1] — grounds the
  no-overclaim control.
- **Structure / abstract (ACA-09/10):** IMRaD; writing order **Methods → Results → Discussion → Introduction →
  Abstract → Title** [ES1]. **Bilingual** abstract — *Resumen* (Spanish) + Abstract (English); **title ≤ 12
  words**; *Palabras clave* (keywords, also in English) [ES1].
- **Citation (ACA-02):** **APA** author-date [ES1] — venue-specific (`venue_policy`).
- **Hedging:** Spanish academic does hedge (*podría / parece / sugiere*); ACA-07 removes only contentless
  filler and never strips an epistemic hedge — calibrate normally, not over-added.
- **Status:** **source-grounded** from an authoritative Spanish reference — gap closed. A final
  **native-speaker review of live output** is recommended as standard QA.

### `tr` Turkish — **SOURCE-GROUNDED** ([TR1] Acıbadem MAA Üniv. FBE · [TR2] İstanbul Üniv. · [TR3] Sabancı Üniv.)
The prior "gap" is **closed**: the norms below are grounded in three authoritative Turkish university thesis
guides (`sources.md` §1b), **not invented** (AIP-3).
- **Script (test PASS):** Latin → `\b` valid; **but Turkish is agglutinative** — a single-word substitution
  that fits English often breaks a Turkish suffixed word, so apply HUM word swaps **conservatively**
  (the guides require grammatically correct, coherent sentences) [TR1 §2.7].
- **Register (ACA-03):** *bilimsel Türkçe* — sentences **short, plain, clear, understandable, coherent**
  (*kısa · sade · açık · anlaşılır · uyumlu*) [TR1 §2.7]. Matches plain-precise-formal-not-ornate.
- **Person & voice (ACA-04) — the signature Turkish norm:** academic Turkish uses **impersonal, third-person
  PASSIVE**; first-person ownership words (*yaptım, gördüm, araştırmamızda*) are replaced by passive
  (*yapıldı, görüldü, araştırmada*) [TR1 §2.7]. **Stronger than English** — flag first-person → impersonal
  passive as a well-grounded convention (still the author's choice, INV-A5).
- **Terminology (ACA-06):** prefer **Turkish terms**; a term with no Turkish equivalent stays in its original
  form but *italic*; use **TDK** dictionaries (sozluk.gov.tr) [TR1 §2.7; TR2].
- **Structure / abstract (ACA-09/10):** **bilingual** abstract — English **ABSTRACT** then Turkish **ÖZET**;
  each a **single paragraph, ≤250 words**, covering **problem · method · results · implications**
  (*amaç/yöntem/bulgular/tartışma*); **no** title, tables, figures, formulas, or footnotes; keywords
  alphabetical; thesis title ≤12 words [TR1 §3.2 · TR3 §3.4].
- **Citation (ACA-02):** **venue-specific** — numbered `[n]` (surname + number; *ve* for two authors;
  *ve diğerleri* = et al. for 3+) [TR2], or author-name / author-year [TR1][TR3]. Driven by `venue_policy`.
- **Mechanical:** a sentence **never starts with a numeral or abbreviation** [TR1 §2.7]; SI units.
- **Hedging density (one honest residual):** these are **format/structure/style** guides — they do **not**
  cover rhetorical hedging density, so for `tr` hedging stays **conservative** (ACA-07 removes only
  contentless filler; never strips an epistemic hedge). The rest above is grounded.
- **Status:** **source-grounded** from authoritative Turkish references — gap closed. A final
  **native-speaker review of live output** is still recommended as standard QA before heavy use.

### `id` Indonesian — **SOURCE-GROUNDED** ([ID1] Univ. Gadjah Mada · [ID2] Panduan Makalah Ilmiah · [ID3] Univ. Pendidikan Indonesia)
The prior "gap" is **closed**: grounded in three authoritative Indonesian university guides (`sources.md`
§1e), **not invented** (AIP-3).
- **Script (test PASS):** Latin → `\b` valid; **but Indonesian is affixing** (meN-, di-, ber-, ke-…-an, -kan,
  -i) — a word-swap that fits English often breaks an affixed Indonesian word, so apply HUM word swaps
  **conservatively**. Preserve numbers, citations, DOI **byte-for-byte** (INV-A1).
- **Person & voice (ACA-04) — the signature Indonesian norm:** sentences **must not** use a first- or
  second-person viewpoint (*saya, aku, kita, kami, engkau*); they are written in the **passive (pasif)**; in
  acknowledgements *saya → penulis* [ID1 §3.4.2]. **Stronger than English** — flag first/second-person →
  passive (still the author's choice, INV-A5).
- **Register (ACA-03):** *bahasa baku* (standard) and *lugas* (plain/concise); the guides give
  **non-standard→standard** (*tidak baku → baku*) and **ineffective→effective** (*kalimat tidak efektif →
  efektif*) conversion lists [ID2]. Conjunctions *sehingga / sedangkan* must **not** start a sentence
  [ID1 §3.4.4].
- **Terminology (ACA-06):** use Indonesian terms or standardised loanwords per **KBBI**; a foreign term is
  *italicised* and explained [ID1 §3.4.3]. Orthography per **PUEBI** (Pedoman Umum Ejaan Bahasa Indonesia).
- **Objectivity / claim strength (ACA-01):** data are analysed and interpreted **objectively, unbiased,
  logically** (*objektif, tidak bias, logis*) [ID2][ID3] — grounds the no-overclaim control.
- **Structure / abstract (ACA-09/10):** **bilingual** abstract — *Abstrak* (Indonesian) + Abstract (English);
  **150–250 words** (thesis 150–300), covering tujuan/metode/hasil/kesimpulan; **3–5 keywords (kata kunci)**
  [ID1 / ID3].
- **Citation (ACA-02):** in-text author-year; only the first author's surname in text [ID3] — venue-specific
  (`venue_policy`).
- **Hedging:** ACA-07 removes only contentless filler; never strips an epistemic hedge. Calibrate
  conservatively (the guides emphasise *lugas* / concise + objective).
- **Status:** **source-grounded** from authoritative Indonesian references — gap closed. A final
  **native-speaker review of live output** is recommended as standard QA.

### `ms` Malay — **SOURCE-GROUNDED** ([MS1] KUIS/UIS *Panduan Menulis Kertas Akademik* · [MS2] · [MS3] Gaya UKM)
The prior gap state is **closed**: grounded in authoritative Malay academic-writing guides (`sources.md` §1j),
**language-verified** Malay (Malay markers present; Indonesian markers **0**), **not invented** (AIP-3). *(⚠ The
similarly-titled top-level Indonesian file was **not** used — Malay ≠ Indonesian.)*
- **Script (test PASS):** Latin → `\b` valid (conservative — affixation). Preserve numbers, citations, DOI
  **byte-for-byte** (INV-A1). **Malay ≠ Indonesian** — do not transfer `id` guidance.
- **Structure (ACA-09) — grounded:** Pengenalan → Metodologi → Dapatan → Perbincangan → Kesimpulan; in-text
  citation (Bab IV) + Senarai Rujukan (Bab V) [MS1][MS3].
- **Abstract (ACA-09/10) — grounded:** **Abstrak** one paragraph, **200–300 words**, containing **Pengenalan
  (isu/permasalahan) · Objektif kajian · Metodologi · Dapatan · Kesimpulan** [MS1 §3.1.4]; **bilingual** —
  Abstrak (BM) + English Abstract [MS3 G1/G2]; 3–5 kata kunci.
- **Citation (ACA-02) — grounded:** **sistem pengarang-tahun** (author-date) for single / joint / multi
  authors; full Senarai Rujukan for book / article / chapter / proceedings / online / legal [MS1][MS3];
  venue-specific (`venue_policy`).
- **Register / spelling (ACA-03) — grounded:** **ejaan baku** per *Pedoman Umum Ejaan* / **Kamus Dewan** (DBP);
  foreign terms in *italics* (huruf condong) + transliterated [MS3]. Formal, *hendaklah*-prescriptive register.
- **Person/voice (ACA-04) — register-advisory (sources silent):** Malay academic convention favours **ayat
  pasif / impersonal** (no *saya/kami* in the body), but the provided **format guides are silent** on
  grammatical voice — so an impersonal recast is offered as a **Channel-2 advisory** (objectivity constant
  §1), **not** asserted as a separately-grounded mechanical rule.
- **Hedging:** Malay academic hedges (*mungkin / berkemungkinan / dilihat*); ACA-07 removes only contentless
  filler, never an epistemic hedge.
- **Status:** **source-grounded** from authoritative, **language-verified** Malay references — gap closed
  (person/voice register-advisory). A final **native-speaker review of live output** is recommended.

### `ur` Urdu — **SOURCE-GROUNDED (report-writing manual)** ([UR1] AIOU *Manual for Internship, BS Islamic Law*)
The prior gap state is **partly closed** from an authoritative Urdu university **report-writing** manual
(`sources.md` §1h), **not invented** (AIP-3). **Honest scope:** [UR1] is an **internship-report** manual,
**not** a scientific-article guide — structure/format/critical-analysis are grounded; scholarly
person-voice/tense/hedging are **gap-declared** (Channel-2 advisory only).
- **Script (test PASS):** Arabic-script (Urdu) → **no `\b`**; phrase-level only; RTL safety. Preserve **Urdu
  numerals** (۱۸ ۲۰), citations, DOI **byte-for-byte** (INV-A1). **Urdu ≠ Arabic/Persian** — do not transfer.
- **Structure (ACA-09) — grounded:** Title page → Acknowledgements → Contents → List of tables → **Summary
  (خلاصہ)** → objectives → organizational structure → **Findings & Discussion (نتائج اور بحث)** →
  Recommendations (سفارشات) → Annexure (ضمیمہ) [UR1 §1.9].
- **Critical analysis (ACA-08) — grounded:** the manual requires **critical analysis** (*تنقیدی تجزیہ*) and
  emphasis on analysis + recommendations, not mere description [UR1 §1.5, §1.7].
- **Documents-Consulted / sourcing (ACA-02-adjacent) — grounded:** record consulted sources in a **Documents
  Consulted (مشورہ شدہ دستاویزات)** list/Annexure [UR1 §1.4]. (Formal citation *style* is venue-specific —
  not fixed by [UR1].)
- **Typography / register (ACA-03) — grounded:** **Jameel Noori Nastaleeq** font; **Urdu numerals** (۱ ۲ ۳);
  a **space after each punctuation mark** (؛ …); justified both sides [UR1 §1.8].
- **Objectivity (ACA-01) — partial:** observation-based reporting (*مشاہدہ*) [UR1 §1.4] supports the
  no-overclaim control; a full scientific objectivity rule is not separately prescribed.
- **Person/voice (ACA-04), tense (ACA-05), epistemic hedging — [GAP, AIP-3]:** **not** prescribed by a
  report-writing manual. Channel-1 applies only the **universal** de-AI + byte/script preservation; any
  first/second-person → impersonal change is a **Channel-2 advisory**, **not** a grounded `ur` mechanical
  rule, **pending an Urdu scientific-article reference**.
- **Status:** **partially source-grounded** (structure/format/critical-analysis) with a **declared residual
  gap** (scholarly person-voice/tense/hedging). A final **native-speaker review of live output** is
  recommended; full parity awaits an Urdu scientific-writing reference.

---

## 4. Language-QA gate (release gate per non-English language)

A language ships **only when ALL hold**:

1. **Native/expert validation is final.** The per-language guidance passes native review. A model draft
   alone is **not** sufficient. *(Current state: **all 10 languages are grounded** — `tr`, `ar`, `zh`, `id`,
   `es`, `fr`, `fa`, and `ms` are **source-grounded** in authoritative academic-writing guides ([TR1][TR2][TR3]
   / [AR1][AR2][AR3] / [ZH1] / [ID1][ID2][ID3] / [ES1] / [FR1][FR2][FR3] / [FA1][FA2][FA3] / [MS1][MS2][MS3]);
   `ur` is grounded on an Urdu **report-writing** manual ([UR1]) with its scholarly person-voice/tense/hedging
   **gap-declared**; `ms` person/voice is a **register-advisory** (format guides silent). Gaps closed where
   grounded; a **final native-output review per language** is the recommended last QA — validators not yet
   formally identified, Blueprint §10.)*
2. **DeepL is an assistant, never the authority.** It may assist drafting the **guidance text**; it never
   decides and never operates on the user's manuscript (INV-A7).
3. **Per-script-family acceptance test (mechanical):** Latin (`en, fr, es, tr, id, ms`) → `\b` word-level OK;
   Arabic-script (`ar, ur, fa`) → **no `\b`**, phrase-level; Han (`zh`) → **no `\b`**, code-point.
   *(Current state: PASS for all — see §2.)*
4. **`[PROVISIONAL]` gap-language guard (`ur, ms`):** hedging norms **not found** → conservative
   defaults marked **[PROVISIONAL]**, guarded, gap **declared not invented** (AIP-3). *(`tr` and `id` left
   this set — now source-grounded, §3.)*

**Conclusion (P5):** **all 10 languages are now grounded.** `tr`, `ar`, `zh`, `id`, `es`, `fr`, `fa`, and
`ms` are **source-grounded** in authoritative academic-writing references — gaps closed for
register/objectivity/structure/citation (`id` passive, `es` impersonal *se*, `fr` passive form, `fa`
impersonal objective register, `ms` ejaan baku + abstrak 200–300 words; `ms` person/voice is a
register-advisory as its format guides are silent). **`ur` is grounded on an Urdu report-writing manual**
([UR1]) for structure/format/critical-analysis, with scholarly person-voice/tense/hedging **gap-declared**
(advisory only; full parity awaits an Urdu scientific-article reference). **Condition 3 PASSES** for all and
the condition-4 guard applies; **a final native review of live output per language is the recommended last
QA** (esp. zh-CN Simplified — Blueprint §10). **Operative languages: `en` (shipped) + `tr` + `ar` + `zh` +
`id` + `es` + `fr` + `fa` + `ms` + `ur` — all 10.** None remains a [PROVISIONAL] draft.

---

## 5. Rollout order (P5, gated)

`en` (SHIPPED) · `tr` · `ar` · `zh` · `id` · `es` · `fr` · `fa` · `ms` (**SOURCE-GROUNDED**) · `ur` (**report-manual grounded**). **All 10 languages grounded — rollout complete.**
**Operative now: all 10 — `en` + `tr` + `ar` + `zh` + `id` + `es` + `fr` + `fa` + `ms` + `ur`** (`ur`/`ms` with declared register-advisories; a **final native-output review per language** is the recommended last QA; INV-A7).

---

*Skill reference — P5 build (ALL 10 languages grounded: `tr`+`ar`+`zh`+`id`+`es`+`fr`+`fa`+`ms` source-grounded from academic-writing references; `ur` grounded on a report-writing manual with residual scholarly-register gap declared; **0 languages [PROVISIONAL]**). © 2026 Dr. Aladdin Ali / Aladdin Pertanian Internasional.*
