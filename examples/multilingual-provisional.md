<!--
Copyright (c) 2026 Dr. Aladdin Ali - Founder of Aladdin Pertanian Internasional - dr.alaa@aladdin.my.id. All Rights Reserved.
-->

# Multilingual Examples — [PROVISIONAL], native-validation PENDING
## Skill reference — P5 build · NOT shipped

> **⚠ Provisional drafts.** These illustrate **only** the **language-agnostic, English-validated** behaviours
> — universal de-AI removals (sycophancy `HUM-22`, emoji `HUM-18`), **byte-for-byte preservation** of
> numbers/citations/DOIs (INV-A1), and **script-family handling** (no `\b` for Arabic-script/Han). They do
> **NOT** demonstrate validated register/hedging on their own — but **all nine non-English languages are now
> grounded** elsewhere: `tr`/`ar`/`zh`/`id`/`es`/`fr`/`fa`/`ms` are **SOURCE-GROUNDED** and `ur` is
> **report-manual grounded** (scholarly person-voice **gap-declared**) — see `languages.md` §3 + `sources.md`
> §1b–§1j; full worked examples in `before-after.{tr,ar,zh,id,es,fr,fa,ms,ur}.md`. The entries below are
> **quick illustrations** pointing to those full examples. **All 10 languages operative; a final native-output
> review per language is the recommended last QA (INV-A7).**
> The three-channel model and the consent gate are **identical to English** — see
> [before-after.md](before-after.md). Each input carries a sycophantic opener + an emoji + `18 of 20` + a
> table ref + `[3]`; Channel 1 removes the AI tells and **preserves every number and citation**.

---

### `ar` Arabic — **SOURCE-GROUNDED** ([AR1] · Arabic-script · no `\b` · phrase-level)
- **Input:** "هذه نتيجة رائعة! 😊 في تجربتنا، استجاب **18 من 20** مريضًا (انظر **الجدول 1**) **[3]**."
- **Channel 1 (de-AI + grounded voice):** "في التجربة، استجاب **18 من 20** مريضًا (انظر **الجدول 1**) **[3]**."
- *Removed:* "هذه نتيجة رائعة! 😊" (HUM-22 + HUM-18). **Grounded person rule (ACA-04 · [AR1]):** first-person
  *في تجربتنا* (in **our** experiment) → impersonal *في التجربة*; no personal pronouns. *Preserved:*
  `18 من 20` · `الجدول 1` · `[3]`; no `\b` (phrase-level), RTL number-unit intact.
  → **أمثلة مُنفَّذة كاملة (English parity):** [before-after.ar.md](before-after.ar.md).

### `zh` Chinese — **SOURCE-GROUNDED** ([ZH1] · Han · no `\b` · code-point)
- **Input:** "这个结果太棒了！😊 在我们的试验中，**20** 名患者中有 **18** 名做出了反应（见**表 1**）**[3]**。"
- **Channel 1 (de-AI + grounded voice):** "在本试验中，**20** 名患者中有 **18** 名做出了反应（见**表 1**）**[3]**。"
- *Removed:* "这个结果太棒了！😊" (HUM-22 + HUM-18). **Grounded person rule (ACA-04 · [ZH1] §16.3.1):** avoid
  the personal pronoun *我们* (we) → definite *本试验* (this trial). *Preserved:* `20` · `18` · `表 1` ·
  `[3]`; code-point, no word-boundary substitution.
  → **完整範例 (English parity):** [before-after.zh.md](before-after.zh.md).

### `fa` Persian — **SOURCE-GROUNDED** ([FA1] · Arabic-script · no `\b` · phrase-level)
- **Input:** "این نتیجه عالی است! 😊 در آزمایش ما، **۱۸ از ۲۰** بیمار پاسخ دادند (**جدول ۱**) **[3]**."
- **Channel 1 (de-AI + grounded voice):** "در این آزمایش، **۱۸ از ۲۰** بیمار پاسخ دادند (**جدول ۱**) **[3]**."
- *Removed:* "این نتیجه عالی است! 😊" (HUM-22 + HUM-18). **Grounded register rule (ACA-01/ACA-04 · [FA1]):**
  subjective first-person *آزمایش ما* (our trial) → impersonal *این آزمایش*; academic Persian is
  **objective/impartial (بی‌طرفانه)** and personal/subjective appeals «have no place». *Preserved:*
  `۱۸ از ۲۰` · `جدول ۱` · `[3]`; **Persian digits byte-for-byte**; no `\b`. **Persian ≠ Arabic**.
  → **نمونه‌های کامل (English parity):** [before-after.fa.md](before-after.fa.md).

### `fr` French — **SOURCE-GROUNDED** ([FR2] · Latin · `\b` word-level)
- **Input:** "Ce résultat est vraiment génial ! 😊 Dans notre essai, **18 patients sur 20** ont répondu (voir **Tableau 1**) **[3]**."
- **Channel 1 (de-AI + grounded voice):** "Dans l'essai, **18 patients sur 20** ont répondu (voir **Tableau 1**) **[3]**."
- *Removed:* "Ce résultat est vraiment génial ! 😊" (HUM-22 + HUM-18). **Grounded voice rule (ACA-04 · [FR2]):**
  first-person *notre essai* (our trial) → impersonal *l'essai*; the **passive form** is recommended in French
  scientific writing. *Preserved:* `18 … sur 20` · `Tableau 1` · `[3]`.
  → **Exemples complets (English parity):** [before-after.fr.md](before-after.fr.md).

### `es` Spanish — **SOURCE-GROUNDED** ([ES1] · Latin · `\b` word-level)
- **Input:** "¡Este resultado es realmente genial! 😊 En nuestro ensayo, **18 de 20** pacientes respondieron (véase la **Tabla 1**) **[3]**."
- **Channel 1 (de-AI + grounded voice):** "En el ensayo, **18 de 20** pacientes respondieron (véase la **Tabla 1**) **[3]**."
- *Removed:* "¡Este resultado es realmente genial! 😊" (HUM-22 + HUM-18). **Grounded voice rule (ACA-04 ·
  [ES1]):** first-person *nuestro ensayo* (our trial) → impersonal *el ensayo*; academic Spanish uses the
  impersonal/passive *se*. *Preserved:* `18 de 20` · `Tabla 1` · `[3]`.
  → **Ejemplos completos (English parity):** [before-after.es.md](before-after.es.md).

### `tr` Turkish — **SOURCE-GROUNDED** ([TR1] §2.7 · Latin · `\b` conservative — agglutinative)
- **Input:** "Bu sonuç gerçekten harika! 😊 **Araştırmamızda 20** hastanın **18**'inde yanıt **gözlemledik** (bkz. **Tablo 1**) **[3]**."
- **Channel 1 (de-AI + grounded voice):** "**Araştırmada 20** hastanın **18**'inde yanıt **gözlemlendi** (bkz. **Tablo 1**) **[3]**."
- *Removed:* "Bu sonuç gerçekten harika! 😊" (HUM-22 + HUM-18). **Grounded person rule (ACA-04 · [TR1] §2.7):**
  first-person *Araştırmamızda … gözlemledik* (in **our** research **we** observed) → impersonal passive
  *Araştırmada … gözlemlendi* (in the research it **was** observed). *Preserved:* `20` · `18` · `Tablo 1` ·
  `[3]`. *Hedging density:* conservative for `tr` (not covered by the format guides).
  → **Tam çalışılmış örnekler (English parity):** [before-after.tr.md](before-after.tr.md).

### `id` Indonesian — **SOURCE-GROUNDED** ([ID1] §3.4.2 · Latin · `\b` conservative — affixation)
- **Input:** "Hasil ini benar-benar luar biasa! 😊 Dalam uji coba kami, **18 dari 20** pasien merespons (lihat **Tabel 1**) **[3]**."
- **Channel 1 (de-AI + grounded voice):** "Dalam uji coba ini, **18 dari 20** pasien merespons (lihat **Tabel 1**) **[3]**."
- *Removed:* "Hasil ini benar-benar luar biasa! 😊" (HUM-22 + HUM-18). **Grounded person rule (ACA-04 · [ID1]
  §3.4.2):** first-person *uji coba kami* (our trial) → impersonal *uji coba ini*; no first/second person —
  passive. *Preserved:* `18 dari 20` · `Tabel 1` · `[3]`.
  → **Contoh lengkap (English parity):** [before-after.id.md](before-after.id.md).

### `ms` Malay — **SOURCE-GROUNDED** ([MS1] · Latin · `\b` · language-verified)
- **Input:** "Keputusan ini sungguh hebat! 😊 Dalam ujian kami, **18 daripada 20** pesakit memberi respons (lihat **Jadual 1**) **[3]**."
- **Channel 1 (de-AI; universal):** "Dalam ujian kami, **18 daripada 20** pesakit memberi respons (lihat **Jadual 1**) **[3]**."
- *Removed:* "Keputusan ini sungguh hebat! 😊" (HUM-22 + HUM-18). **Person/voice (ACA-04) — [register-advisory]:**
  [MS1]/[MS3] are **format** guides, silent on grammatical voice; Malay convention favours **ayat pasif**
  (impersonal), offered as a Channel-2 advisory — first-person *ujian kami* kept in Channel 1. *Preserved:*
  `18 daripada 20` · `Jadual 1` · `[3]`. **Malay ≠ Indonesian** (language-verified).
  → **Contoh penuh (English parity):** [before-after.ms.md](before-after.ms.md).

### `ur` Urdu — **SOURCE-GROUNDED (report manual)** ([UR1] · Arabic-script · no `\b` · phrase-level)
- **Input:** "یہ نتیجہ واقعی شاندار ہے! 😊 ہمارے تجربے میں، **۲۰ میں سے ۱۸** مریضوں نے جواب دیا (**جدول ۱** دیکھیں) **[3]**."
- **Channel 1 (de-AI; universal):** "ہمارے تجربے میں، **۲۰ میں سے ۱۸** مریضوں نے جواب دیا (**جدول ۱** دیکھیں) **[3]**."
- *Removed:* "یہ نتیجہ واقعی شاندار ہے! 😊" (HUM-22 + HUM-18). **Person/voice (ACA-04) — [GAP, advisory]:** [UR1]
  is a **report-writing** manual; it does **not** prescribe Urdu scholarly person-voice, so *ہمارے تجربے*
  (our trial) is **kept** in Channel 1 — any impersonal change is a **Channel-2 advisory**, not a grounded
  rule. *Preserved:* `۲۰ میں سے ۱۸` · `جدول ۱` · `[3]`; **Urdu numerals byte-for-byte**; no `\b`
  (phrase-level). **Urdu ≠ Arabic/Persian**.
  → **مکمل مثالیں (English parity):** [before-after.ur.md](before-after.ur.md).

---

**Status:** **all nine non-English languages are now grounded** — `tr`/`ar`/`zh`/`id`/`es`/`fr`/`fa`/`ms` are
**source-grounded** (academic-writing references) and `ur` is **grounded on a report-writing manual** [UR1]
(scholarly person-voice/tense/hedging **gap-declared**; `ms` person/voice register-advisory). The entries
above are **quick illustrations** — the full grounded worked examples are `before-after.<lang>.md`. **All 10
languages are operative; a final native-output review per language is the recommended last QA (INV-A7).**

---

*Skill reference — P5 build (provisional). © 2026 Dr. Aladdin Ali / Aladdin Pertanian Internasional.*
