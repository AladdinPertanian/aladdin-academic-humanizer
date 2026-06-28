<!--
Copyright (c) 2026 Dr. Aladdin Ali - Founder of Aladdin Pertanian Internasional - dr.alaa@aladdin.my.id. All Rights Reserved.
-->

# Source Manifest
## Skill reference — P4 build
### `filename · title · URL · access_date · sha256 · license` (Blueprint §2.4)

> **Verifiability (gate G2).** The 4 primary PDFs carry a **recomputable source-side sha256** (recomputed
> 2026-06-27 — matches Blueprint Appendix B). Web rows marked **[specific]** carry a verified deep link; the
> rest are domain-only (dated re-verification deferred to §10).
> **Bundling — Option B (adopted 2026-06-27, final).** The PDFs are **referenced, not bundled** — the Owner
> does **not** hold redistribution rights — so this manifest carries the **source-side** checksum
> (recomputable at `aladdin-pertanian-agri-ai/docs/Marketing/pdf/`). This is the adopted approach, **not** a
> pending divergence; G2 is therefore verified **source-side**.
> **Point-in-time.** Web policies evolve; a **dated re-verification before release** remains open
> (Blueprint §10 / §9 #7).

---

## 1. Primary sources (owner-provided PDFs) — source-side sha256 recomputed 2026-06-27

| tag | filename | title | bytes | sha256 | license / use |
|-----|----------|-------|------:|--------|---------------|
| `[Q]` | Guide-of-writing-academic-thesis-Qassim-University-1.pdf | Qassim University — *Guide to Preparing and Writing an Academic Thesis* (MSc CS, 2024) | 612534 | `c97eb85a3cecf59d0fe35ddf72daea0f3e88b8ead3e5225dcc692f633f73e52d` | © author/institution — reference use (referenced, not redistributed — Option B) |
| `[T]` | how-to-write-master-thesis-torresen.pdf | J. Tørresen — *How to Write a Master's Thesis* (Univ. of Oslo, Informatics) | 178358 | `6393ce5879994783ea009a4a69f511852ca0616d720dbdd4095b77523a0e386d` | © author/institution — reference use (referenced, not redistributed — Option B) |
| `[ART]` | Writing_a_scientific_article__A_step-by-step_guide_for_beginners_.pdf | Ecarnot F. et al. — *Writing a scientific article: a step-by-step guide for beginners*, Eur. Geriatr. Med. (2015) | 676575 | `98e2e4ab922d6ed678db5112f2d2b4ebdcd649ce7c9338792ce0fc00cbbb562e` | © author/publisher — reference use (referenced, not redistributed — Option B) |
| `[THE]` | writing_a_scientific_thesis.pdf | D. Burns — *Writing a Scientific-Style Thesis*, NUI Galway (2017) | 2761021 | `9911b22b622e82d36bdd70edd9b7de44f38b99e3c411e16c999fe0c0d30fc0b3` | © author/institution — reference use (referenced, not redistributed — Option B) |

*Verification: `sha256sum` of each file at `aladdin-pertanian-agri-ai/docs/Marketing/pdf/` reproduces the
hash above — this source-side hash is **authoritative** under Option B. (If redistribution rights are ever
confirmed, a bundled copy could be added later with its own checksum; that is not planned.)*

### 1b. Turkish-language references (ground `tr` — see `languages.md`) — sha256 recomputed 2026-06-27

| tag | filename | source / institution | bytes | sha256 | license / use |
|-----|----------|----------------------|------:|--------|---------------|
| `[TR1]` | fbe-tez-yazim-kilavuzu.pdf | Acıbadem Mehmet Ali Aydınlar Üniversitesi — Fen Bilimleri Enstitüsü, *Tez Yazım Kılavuzu* (§2.7 Anlatım, Özet, terminology) | 937887 | `bfef9047e7cbe5cdb2fe9d21f80d1049a314cff42e599b815a13705c1b9118a2` | © institution — reference use (referenced, not redistributed — Option B) |
| `[TR2]` | tez-yazim-kilavuzu_yl.pdf | İstanbul Üniversitesi — Havacılık Psikolojisi Araştırmaları Enstitüsü, *Yüksek Lisans Tez Yazım Kılavuzu* (numbered citation; TDK orthography) | 1448082 | `6137ac354a12ebc6d8c2676073ca86379b93cbd40b3fb03a5f45374b14202c7b` | © institution — reference use (referenced, not redistributed — Option B) |
| `[TR3]` | handbook-11th-revision-fall-2025_tr.pdf | Sabancı Üniversitesi — *Tez Yazım Kılavuzu* (11th revision, Fall 2025) — bilingual Abstract/Özet (mandatory) | 2275694 | `10a3ddd09726741d89b4b2c18f6ea0bba4c59f2d309f9b97fde76a25f49d5582` | © institution — reference use (referenced, not redistributed — Option B) |

*These three authoritative Turkish university thesis guides **source-ground** the `tr` register/person/structure/
terminology/citation/orthography norms (`languages.md` §3), **closing the prior `tr` "gap"** (AIP-3 — norms
now found in trusted sources, not invented). They do **not** cover rhetorical hedging density — that stays
conservative for `tr`. Located at `aladdin-pertanian-agri-ai/docs/Marketing/pdf/tr/`.*

### 1c. Arabic-language references (ground `ar` — see `languages.md`) — sha256 computed 2026-06-28

| tag | filename | source / institution | bytes | sha256 | license / use |
|-----|----------|----------------------|------:|--------|---------------|
| `[AR1]` | دليل اعداد وكتابة الرسائل العلمية.pdf | **جامعة قناة السويس (Suez Canal Univ.)** — *دليل إعداد وكتابة الرسائل العلمية* (passive/third-person voice + tense + scientific register + objectivity + abstract) | 1998590 | `9b01f295519aec7d5bf838fb7118d172114e82865afb2d87992dc2ce6a4533ba` | © institution — reference use (referenced, not redistributed — Option B) |
| `[AR2]` | كلية الاقتصاد بجامعة الملك عبد العزيز.pdf | **King Abdulaziz Univ. — Faculty of Economics & Administration** — *دليل كتابة الرسائل العلمية* (formatting · الاقتباس · bilingual المستخلص ≤200 words) | 932771 | `f1eb7b31e95260080a13880a5137f76a2e470a48d13bdb0882d840b86e4f84ff` | © institution — reference use (referenced, not redistributed — Option B) |
| `[AR3]` | دليل_إعداد_الرسائل_العلمية_والمشروعات_البحثية.pdf | **عمادة الدراسات العليا** — *دليل إعداد الرسائل العلمية والمشروعات البحثية* (الموضوعية/المنهجية + detailed التوثيق rules) | 4466657 | `a42d319684d693b45159dde10303104df48f22731a5a626f33e939675630b5b4` | © institution — reference use (referenced, not redistributed — Option B) |

*These three authoritative Arabic university thesis guides **source-ground** the `ar` register / person-voice /
tense / structure / citation norms (`languages.md` §3), **closing the prior `ar` directional-provisional
state** (AIP-3). The folder also holds the Qassim guide (= `[Q]` in §1 — already a primary source). Arabic
academic register is **more direct than English**, and the guides explicitly require **passive / third-person
voice with no personal pronouns** (with the example: "Do not write 'We measured…' → 'The … was measured'").
Located at `aladdin-pertanian-agri-ai/docs/Marketing/pdf/ar/`.*

### 1d. Chinese-language reference (ground `zh` — see `languages.md`) — sha256 computed 2026-06-28

| tag | filename | source | bytes | sha256 | license / use |
|-----|----------|--------|------:|--------|---------------|
| `[ZH1]` | Academic paper writing instruction_zh.pdf | *學術研究論文撰寫說明* — Academic Research Paper Writing Instructions (Traditional Chinese, 181 pp): §16.3 no-colloquial / no-personal-pronouns · §16.2 objectivity · §16.5 in-text citation · §16.6–16.7 abstract + keywords | 3938415 | `67a65b21d38f1dc1acc974da39e9c8465b4f81dec0ed6b44596a2279ae46cf63` | © author/institution — reference use (referenced, not redistributed — Option B) |

*This authoritative Chinese academic-writing guide **source-grounds** the `zh` register / person-voice /
objectivity / structure / citation norms (`languages.md` §3), **closing the prior `zh` directional-provisional
state** (AIP-3). §16.3 gives a concrete **colloquial→formal** list (如果→若 · 所以→故 · 等等→等 · avoid the
discourse-marker fillers 來說 / 換句話說 / 也就是說 · avoid 自問自答 self-Q&A · **avoid personal pronouns
我 / 我們 / 你**, use definite nouns / 本研究) that directly instantiates the de-AI / ACA patterns in Chinese.
**Source is Traditional Chinese (繁體)**; the register/person/objectivity principles apply to academic Chinese
broadly, but Simplified-specific conventions (zh-CN) warrant a native check. Located at
`aladdin-pertanian-agri-ai/docs/Marketing/pdf/`.*

### 1e. Indonesian-language references (ground `id` — see `languages.md`) — sha256 computed 2026-06-28

| tag | filename | source / institution | bytes | sha256 | license / use |
|-----|----------|----------------------|------:|--------|---------------|
| `[ID1]` | PEDOMAN-PENULISAN-KARYA-ILMIAH-Versi-cetak-2016.pdf | **Universitas Gadjah Mada** — *Pedoman Penulisan Karya Ilmiah* (2016) — §3.4.2 passive / no first-or-second person · §3.4.3 terms (KBBI) · PUEBI spelling · §3.4.4 common errors | 6782753 | `30c7a51768364d5f3365e234a7a9e9875408f2a1846b32c9ca412260fe7b9617` | © institution — reference use (referenced, not redistributed — Option B) |
| `[ID2]` | Panduan Penulisan Makalah Ilmiah.pdf | *Panduan Penulisan Makalah Ilmiah* — objectivity (objektif, tidak bias) · non-standard→standard (baku) & ineffective→effective (kalimat efektif) tables · concise (lugas) verbs | 7085301 | `ba6c3610961e1b9ac8ee2c00da28c9a2678b0552de52db0b3b87904f080b4ec6` | © author/institution — reference use (referenced, not redistributed — Option B) |
| `[ID3]` | Pedoman-Penulisan-Karya-Ilmiah-Tahun-2024.pdf | **Universitas Pendidikan Indonesia** — *Pedoman Penulisan Karya Ilmiah* (2024) — bilingual abstract 150–250 words · 3–5 keywords · citation author-year | 8775470 | `4d589fc7268a895e390c3378f64d8973c90edc26a044fb9a28d36aed61f8b607` | © institution — reference use (referenced, not redistributed — Option B) |

*These three authoritative Indonesian university guides **source-ground** the `id` register / person-voice /
terminology / objectivity / structure / citation norms (`languages.md` §3), **closing the prior `id` "gap"**
(AIP-3 — norms now found in trusted sources). [ID1] §3.4.2: sentences must **not** use first/second person
(*saya/aku/kita/engkau*) — written in the **passive (pasif)**; *saya → penulis*. Located at
`aladdin-pertanian-agri-ai/docs/Marketing/pdf/id/`.*

### 1f. Spanish-language reference (ground `es` — see `languages.md`) — sha256 computed 2026-06-28

| tag | filename | source | bytes | sha256 | license / use |
|-----|----------|--------|------:|--------|---------------|
| `[ES1]` | Manual-de-redacción-de-artículos-científicos_es.pdf | *Manual de redacción de artículos científicos* (university Faculty of Sciences, 69 pp) — impersonal/passive *se* voice · past tense (Methods/Results) · objectivity · IMRaD writing order · bilingual Resumen + Abstract · title ≤ 12 words · APA citation | 1016464 | `79cf4a3ae45a53eeda8df7a6c2d34ab37c2f379372c4d7f809dce5ac86e5ea2f` | © author/institution — reference use (referenced, not redistributed — Option B) |

*This authoritative Spanish scientific-writing manual **source-grounds** the `es` register / person-voice /
tense / objectivity / structure / citation norms (`languages.md` §3), **closing the prior `es`
directional-provisional state** (AIP-3). The manual consistently uses the **impersonal / passive-reflexive
*se*** (*se realizó · se observó · se analizó · se presenta*) and follows **APA** — the Spanish academic
voice norm (no first person). Located at `aladdin-pertanian-agri-ai/docs/Marketing/pdf/`.*

### 1g. French-language references (ground `fr` — see `languages.md`) — sha256 computed 2026-06-28

| tag | filename | source | bytes | sha256 | license / use |
|-----|----------|--------|------:|--------|---------------|
| `[FR1]` | Guide de rédaction des articles scientifiques_2.pdf | *Guide de rédaction des articles scientifiques* (98 pp) — objective/neutral language · résumé 200–400 words bilingual · 5–6 keywords · objective | 1541235 | `03fe5acdfa26c6fa41aedf0dc8f60e5f42308de045029c4749771147ee1f93e0` | © author/institution — reference use (referenced, not redistributed — Option B) |
| `[FR2]` | Guide de rédaction des articles scientifiques_Fr.pdf | **C.F. Boudouresque**, *Manuel de rédaction scientifique et technique* (Éd. 2014-2015, MIO) — ★**passive voice recommended** (je/nous "pas recommandée", on "déconseillé") · terminology (*termes schtroumpf*) · §4.6 Style | 9822927 | `b20f97cfdebeadc69c400cb385aa62d53059678c6a351b54c79ebdcbd9d06cc0` | © author/institution — reference use (referenced, not redistributed — Option B) |
| `[FR3]` | Wegleitung_Anthropos sept2025_FR.pdf | *Wegleitung Anthropos* (Sept 2025) — journal author guidelines (venue-specific citation/format) | 539821 | `9fa177fe62dd05226de89ddef759d2ffa751d53834d54014143df7cdbf2116e1` | © journal — reference use (referenced, not redistributed — Option B) |

*These three authoritative French scientific-writing guides **source-ground** the `fr` register / person-voice /
terminology / objectivity / structure / citation norms (`languages.md` §3), **closing the prior `fr`
directional-provisional state** (AIP-3). [FR2/Boudouresque]: of the four voice options, the **passive form**
(*"Les prélèvements ont été effectués…"*) is the **one recommended** in scientific writing; *je/nous* are not
recommended and *on* is discouraged — the French academic voice norm. Located at
`aladdin-pertanian-agri-ai/docs/Marketing/pdf/fr/`.*

### 1h. Urdu-language reference (ground `ur` — see `languages.md`) — sha256 computed 2026-06-28

| tag | filename | source | bytes | sha256 | license / use |
|-----|----------|--------|------:|--------|---------------|
| `[UR1]` | ur/Manual_2975.pdf | **AIOU** (Allama Iqbal Open University, Islamabad), Dept. of Shariah — *Manual for Internship, BS Islamic Law* (Course 2975, 11 pp; coord. Dr. Tahira Afraq) — report **structure** (Summary خلاصہ · Findings & Discussion نتائج اور بحث · Recommendations · Annexure §1.9) · **critical analysis** (تنقیدی تجزیہ §1.7) · **Documents Consulted** list (مشورہ شدہ دستاویزات §1.4) · Urdu **typography** (Jameel Noori Nastaleeq font · Urdu numerals ۱۲۳ · space after each punctuation · word band §1.8) | 457917 | `f7c95c4ebe8bc711ee09db384e3f9ea431e7562e22d7732d651f9f4137bf7550` | © AIOU — reference use (referenced, not redistributed — Option B) |

> ***Honest scope limit (AIP-3 · PILLAR VII).*** *[UR1] is an **authoritative university report-writing
> manual**. It **source-grounds** the Urdu **document structure / summary / findings-and-discussion /
> critical-analysis / Documents-Consulted / typography** norms (`languages.md` §3). But it is an
> **internship-report** manual, **not** a scientific-article writing guide — it does **not** prescribe
> scholarly **person/voice (ACA-04), tense (ACA-05), or epistemic hedging**. Those are **gap-declared** for
> `ur` (a dedicated Urdu **scientific-article** reference is needed to close them) and are surfaced as
> **Channel-2 advisories**, never asserted as a grounded `ur` norm. Preserve **Urdu numerals** (۱۸ ۲۰)
> byte-for-byte (INV-A1). Located at `aladdin-pertanian-agri-ai/docs/Marketing/pdf/ur/`.*

### 1i. Persian-language references (ground `fa` — see `languages.md`) — sha256 computed 2026-06-28

| tag | filename / URL | source | bytes | sha256 | license / use |
|-----|----------------|--------|------:|--------|---------------|
| `[FA1]` | راهنمای نگارش مقالات دانشگاهی.pdf | *راهنمای نگارش مقالۀ دانشگاهی* (Guide to Writing an Academic Article), **آینۀ پژوهش / Āyene-ye Pažuheš** journal, yr 31 no. 6 (22 pp) — **owner-provided** — **objectivity** (بی‌طرفانه; reason-not-emotion; personal/subjective appeals «جایگاهی ندارند») · **citation** integrity (author-date / author-page / in-text / footnote; under-citation ≈ plagiarism) · style/register · structure · چکیده | 438176 | `8c0767254e02ae56ec1bd01e7fc49a581fd26b65b0d7ec80f61b6ccd53a96365` | © author/journal — reference use (referenced, not redistributed — Option B) |
| `[FA2]` | goums.ac.ir/…/آموزش_مقاله_نویسی…pdf (web, downloaded 2026-06-28) | *آموزش مقاله‌نویسی از ابتدا تا ارسال به مجله* — **Golestan University of Medical Sciences** (39 pp) — **structure** (ساختار مقاله; IMRaD: مقدمه/روش/یافته‌ها/بحث/نتیجه; quantitative vs qualitative) · **methodology reporting** (روش‌شناسی) · **clarity** (روشنی برای خواننده) | 1490633 | `a555fd0c3c2a494a4f573324d6afafc203767b0965e7f30be73e41ef702d6c0f` | © institution — reference use (referenced, not redistributed — Option B) |
| `[FA3]` | cjs.mubabol.ac.ir/page/48 (web, accessed 2026-06-28) | *راهنمای نگارش مقاله* — **Caspian Journal of Scientometrics** — **bilingual** چکیده فارسی + English Abstract (150–250 words) · 3–5 کلیدواژه (Persian + English) | — | — (web; URL + access date) | © journal — reference use |
| `[FA4]` | 1راهنمای نگارش مقالات دانشگاهی.pdf | *نگارش مقاله، گزارش و سایر انتشارات علمی: از انتخاب موضوع تا چاپ* (Writing articles, reports & other scientific publications) — **owner-provided** comprehensive guide (219 pp). **Note:** its PDF text layer is **Arabic presentation-form glyphs** → **not machine-extractable for quotation** here, so no specific norm is attributed to it; listed for authority/completeness. `fa` norms are quoted from [FA1]/[FA2]. | 5134075 | `d8f1f51b3a7f993bb1ab56c438e829393b27262353243020deee0ac82464efc1` | © author/publisher — reference use (referenced, not redistributed — Option B) |

*[FA1] (owner-provided) and [FA2] (university, web — re-downloadable; sha256 above is authoritative under
Option B) **source-ground** the `fa` objectivity / register / citation / structure / abstract norms
(`languages.md` §3), **closing the prior `fa` provisional state** (AIP-3). [FA3] corroborates the **bilingual
Persian + English abstract/keywords** convention. Persian is **Arabic-script** → no `\b`; preserve **Persian
numerals** (۱۸ ۲۰) and the decimal separator (٬/٫) byte-for-byte (INV-A1). [FA1] located at
`aladdin-pertanian-agri-ai/docs/Marketing/pdf/`.*

### 1j. Malay-language references (ground `ms` — see `languages.md`) — sha256 computed 2026-06-28

| tag | filename / URL | source | bytes | sha256 | license / use |
|-----|----------------|--------|------:|--------|---------------|
| `[MS1]` | my/Panduan Menulis Kertas Akademik.1.pdf | **KUIS / UIS** (Kolej Universiti Islam Antarabangsa Selangor / Universiti Islam Selangor), Fakulti Pengajian Peradaban Islam — *Panduan Menulis Kertas Akademik* (2023, 63 pp) — **owner-provided** — structure · **abstrak** (200–300 words: Pengenalan/Objektif/Metodologi/Dapatan/Kesimpulan) · **citation** (sistem pengarang-tahun; senarai rujukan) · ejaan baku | 1075d13a89827882… | © KUIS/UIS — reference use (referenced, not redistributed — Option B) |
| `[MS2]` | my/Panduan Menulis Kertas Akademik.2.pdf | same title — variant edition (68 pp) — **owner-provided** corroborating | 2971fe5fb3be45d9… | © author/institution — reference use (Option B) |
| `[MS3]` | ukm.my/kita/…/GAYA-UKM_BAHASA-MELAYU.pdf (web, downloaded 2026-06-28) | **UKM** *Panduan Penulisan Tesis — Gaya UKM* (Bahasa Melayu, 134 pp) — **bilingual** abstrak BM + English (Lampiran G1/G2) · ejaan baku (Kamus Dewan / DBP) · Gaya UKM citation | `747de80cd7002b4cbb8013179a57377808939d8d6a026ccd0ae63e3b4874b3fb` | © UKM — reference use (Option B) |

> ***Language verified (AIP-3 · PILLAR VII).*** *[MS1]/[MS2] (owner-provided, `pdf/my/`) and [MS3] (UKM, web —
> re-downloadable) are **confirmed Malay** (Malay markers kerana/ialah/hendaklah present; Indonesian markers
> karena/kasus/referensi = **0**) and **source-ground** the `ms` structure / abstract / citation /
> ejaan-register norms (`languages.md` §3), closing the prior `ms` gap. **⚠ The similarly-titled top-level
> `Panduan Menulis Kertas Akademik.df.pdf` is INDONESIAN** (verified: karena/kasus/referensi present,
> kerana/kes/ialah absent, mentions "di Indonesia") — **NOT used for `ms`** (Malay ≠ Indonesian, a documented
> trap). The three Malay guides are **format/structure guides, silent on grammatical person/voice**, so the
> **ayat-pasif / impersonal** preference (ACA-04) is a **register-advisory**, not a separately-grounded
> mechanical rule. Latin → `\b` valid (conservative — affixation). [MS1]/[MS2] at `…/pdf/my/`.*

---

## 2. Web sources

> **Verification status.** Only rows marked **[specific]** carry a verified deep link (point-in-time, from
> the owner Position Statement §6 / Blueprint §2.2). All other rows are **domain-only** here: the exact page
> and a **dated re-verification are deferred to §10** (Blueprint §9 #7) and are **not** asserted as verified.
> No row's access has been re-fetched in this build.

### Integrity & AI policy
| name | URL | role |
|------|-----|------|
| ICMJE — AI use by authors | https://www.icmje.org/recommendations/browse/artificial-intelligence/ai-use-by-authors.html **[specific]** | disclosure + no-AI-authorship |
| COPE — Authorship and AI tools | https://publicationethics.org/guidance/cope-position/authorship-and-ai-tools **[specific]** | authorship position |
| Elsevier — Generative-AI policies for journals | https://www.elsevier.com/about/policies-and-standards/generative-ai-policies-for-journals **[specific]** | author AI-use policy |
| Nature Portfolio — AI editorial policy | https://www.nature.com/nature-portfolio/editorial-policies/ai **[specific]** | editorial policy |
| Taylor & Francis — AI policy | `taylorandfrancis.com` — specific page + dated verification pending (§10) | author policy |
| Wiley — Generative-AI policy (Sept 2023) | `wiley.com` — specific page + dated verification pending (§10) | author policy |

### Detector bias / academic integrity
| name | URL | role |
|------|-----|------|
| Liang et al. (2023) *GPT detectors are biased against non-native English writers*, Patterns 4(7):100779 | https://pmc.ncbi.nlm.nih.gov/articles/PMC10382961 **[specific]** | detector-bias evidence (AIP-5) |
| Vanderbilt — *Academic Integrity and Generative AI* | `vanderbilt.edu` — specific page + dated verification pending (§10) | disabled-detector precedent |
| UNC Writing Center — *Generative AI in Academic Writing* | `writingcenter.unc.edu` — specific page + dated verification pending (§10) | authorship guidance |
| Editors Canada — *Ethical Editing of Graduate Student Texts* | `editors.ca` — specific page + dated verification pending (§10) | editing-ethics |

### Register / hedging / criticality / AI-tells
| name | URL | role |
|------|-----|------|
| Manchester Academic Phrasebank — *Being cautious* | `phrasebank.manchester.ac.uk` — specific page + dated verification pending (§10) | hedging (ACA-07) |
| GMU Writing Center — *Hedges* | `writingcenter.gmu.edu` — specific page + dated verification pending (§10) | hedging (ACA-07) |
| APA Style — *Scholarly tone* / *Bias-free language* | `apastyle.apa.org` — specific page + dated verification pending (§10) | register (ACA-03) |
| Univ. of York — *Criticality* | `york.ac.uk` — specific page + dated verification pending (§10) | criticality (ACA-08) |
| EAP Foundation — *Critical writing* | `eapfoundation.com` — specific page + dated verification pending (§10) | criticality (ACA-08) |
| Wikipedia / WikiProject AI Cleanup — *Signs of AI writing* (CC BY-SA 4.0) | https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing **[specific]** | de-AI **base taxonomy (HUM-01..30)** — HUM-31..33 are Siqi Chen's own MIT additions, not from this article; see [../NOTICE](../NOTICE) |

---

## 3. Notes

- **CC BY-SA 4.0 (Wikipedia)** is **legal-open** in this Skill (Blueprint §7); no share-alike conclusion is
  asserted. The Wikipedia-derived **base taxonomy (HUM-01..30)** is isolated; **HUM-31..33 are Siqi Chen's own
  MIT additions** (not from the article), and the Owner's ACA work is kept separable. See [../NOTICE](../NOTICE).
- The four PDFs evidence the **academic-writing** foundation; the **AI-policy / detector-bias** layer rests
  on the §2 web sources and **must be re-verified (dated snapshots) before release** (Blueprint §9 #7, §10).
- This manifest does not assert redistribution rights for any third-party source.

---

*Skill reference — P4 build. © 2026 Dr. Aladdin Ali / Aladdin Pertanian Internasional.*
