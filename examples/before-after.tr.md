<!--
Copyright (c) 2026 Dr. Aladdin Ali - Founder of Aladdin Pertanian Internasional - dr.alaa@aladdin.my.id. All Rights Reserved.
-->

# Çalışılmış Örnekler (Türkçe) — Worked Examples (Turkish)
## Skill reference — `tr` SOURCE-GROUNDED ([TR1] Acıbadem · [TR2] İstanbul · [TR3] Sabancı)
### English `before-after.md` ile tam paritede / at full parity with the English `before-after.md`

> Bu örnekler `before-after.md` (İngilizce) ile **eşdeğer derinliktedir**. Üç kanal, **revizyon günlüğü** ve
> **onay kapısı** Türkçe olarak gösterilir; her sayı/atıf/DOI **bayt bayt** korunur (INV-A1). Türkçe
> akademik **kişisiz edilgen** kuralı [TR1 §2.7] uygulanır (*araştırmamızda → araştırmada*). Hedging
> yoğunluğu `tr` için **temkinli** kalır (biçim/yapı kılavuzları bunu kapsamaz). Üç kanal modeli ve onay
> kapısı İngilizce ile **birebir aynıdır** (`before-after.md`).

---

## Örnek 1 — Aşırı iddia + de-AI, tam akış (onay verildi)

**Sözleşme:** `level=journal` · `programme_type=journal` · `edit_scope=apply_approved_notes` ·
`co_authored=false` · `ai_disclosure_policy=required` · `output_language=tr`.

**Girdi (Tartışma paragrafı):**
> "Sonuç olarak, çığır açan çalışmamız İlaç X'in kanamaya neden olduğunu açıkça kanıtlıyor! 😊
> Araştırmamızda **20** hastanın **18**'inde kanama gözlemledik (bkz. **Tablo 2**); bu, Almeida ve
> diğerleri **[7]** ile uyumludur."

### Kanal 1 — Dili İyileştirilmiş Metin (otomatik, yalnızca ifade)
> "Çalışma, İlaç X'in kanamaya neden olduğunu açıkça kanıtlıyor. Araştırmada **20** hastanın **18**'inde
> kanama gözlemlendi (bkz. **Tablo 2**); bu, Almeida ve diğerleri **[7]** ile uyumludur."

*Değişen (yalnızca ifade):* "Sonuç olarak," kaldırıldı (HUM-25); "çığır açan" kaldırıldı (HUM-01); "! 😊"
kaldırıldı (HUM-18). **Kişi/çatı kuralı (ACA-04 · [TR1] §2.7):** "çalışmamız" → "çalışma"; birinci kişi
*"Araştırmamızda … gözlemledik"* → edilgen *"Araştırmada … gözlemlendi"*.
*Korunan:* iddia **"açıkça kanıtlıyor … neden olduğunu"** (iddia gücü — bu Kanal 2'dir, ACA-01); ve
**`20` · `18` · `Tablo 2` · `[7]`** — bayt bayt (INV-A1).

### Kanal 2 — Bilimsel Danışma Raporu (önerilir, uygulanmaz)
- **A-01 (ACA-01 · aşırı iddia):** "İlaç X'in kanamaya neden olduğunu açıkça kanıtlıyor" ifadesi tek bir
  18/20 çalışmasının ötesine geçiyor (nedensellik + aşırı genelleme). Önerilen, çalışmaya özgü ve temkinli
  yeniden ifade: *"Bu örneklemde hastaların çoğunda kanama gözlemlendi; bu durum, daha ileri araştırma
  gerektiren bir güvenlik kaygısına işaret edebilir."* *(iddia gücü değişir — karar yazarındır)*

### Yazar onayı
`consent_to_apply = verildi`, kabul edilen: **A-01**; `authorship_acknowledgement = onaylandı`.

### Kanal 3 — Yazar Onaylı Bilimsel Revizyon (uygulandı + insanileştirildi)
> "Çalışma, İlaç X ile kanama arasındaki ilişkiyi incelemektedir. Araştırmada **20** hastanın **18**'inde
> kanama gözlemlendi (bkz. **Tablo 2**); bu durum, daha ileri araştırma gerektiren bir güvenlik kaygısına
> işaret edebilir ve Almeida ve diğerleri **[7]** ile uyumludur."

### Revizyon günlüğü (INV-A10)
**Başlık:** `tr` · `journal`/`journal` · `apply_approved_notes` · `co_authored=false` ·
`ai_disclosure_policy=required` → AI kullanım beyanı eklendi · kabul: `A-01` ·
`authorship_acknowledgement=onaylandı`.

| change_id | konum | kanal | onaylı madde | öncesi → sonrası | gerekçe | değişmez kontrol |
|-----------|-------|:-----:|--------------|------------------|---------|------------------|
| C-001 | Tartışma ¶ | K.3 | A-01 | "İlaç X'in kanamaya neden olduğunu açıkça kanıtlıyor … Araştırmada 20 hastanın 18'inde kanama gözlemlendi → İlaç X ile kanama arasındaki ilişkiyi incelemektedir … bu durum … işaret edebilir" | yazar, çalışmaya özgü temkinli yeniden ifadeyi kabul etti (nedensel aşırı iddia kaldırıldı) | INV-A6: iddia yazar onayıyla daraltıldı; sayılar değişmedi |
| C-002 | Tartışma ¶ | K.1 | — (ACA-04 · [TR1] §2.7) | "Araştırmamızda … gözlemledik → Araştırmada … gözlemlendi" | kişisiz edilgen kuralı (otomatik, anlam korunur) | INV-A6: anlam korundu |
| C-003 | Tartışma ¶ | K.1 | — (HUM-01/18/25) | "Sonuç olarak, çığır açan çalışmamız … ! 😊 → Çalışma …" | yalnızca ifade de-AI | INV-A6: anlam korundu |

**Doğruluk & beyan:** `20` → değişmedi · `18` → değişmedi · `Tablo 2` → değişmedi · `[7]` → değişmedi.
Hiçbir bilimsel sınırlama kaldırılmadı; onaylı madde olmadan zayıf kanıt güçlü iddiaya çevrilmedi. Bildirim:
AI kullanım beyanı eklendi; "tespit edilemez" iddiası yok. **Birincil araştırma sorumluluğu yazarda kalır.**

---

## Örnek 2 — Onay kapısı (onay **verilmedi** → Kanal 3 yok)

**Sözleşme:** `level=masters` · `programme_type=masters_thesis` · `edit_scope=language_clarity` ·
`co_authored=false` · `ai_disclosure_policy=unknown` · `output_language=tr`.

**Girdi:**
> "Şekil 3'te modelin gerçekten pek iyi çalışmadığını açıkça görebilirsiniz; bu, önemli bir sınırlamadır.
> Hata oranı **%12,4**'tü."

### Kanal 1 — Dili İyileştirilmiş Metin (otomatik, yalnızca ifade)
> "Şekil 3, modelin gerçekten pek iyi çalışmadığını göstermektedir; bu, önemli bir sınırlamadır. Hata
> oranı **%12,4**'tü."

*Değişen (yalnızca ifade):* ikinci kişi "Şekil 3'te … görebilirsiniz" → kişisiz "Şekil 3 …
göstermektedir" (ACA-04 · [TR1] §2.7). *Korunan:* yumuşatıcı "gerçekten" (kaldırılması iddia gücünü
artırır → Kanal 2) ve **`%12,4`** — bayt bayt; Türkçe ondalık biçimi (virgül) **değiştirilmez** (INV-A1).

### Kanal 2 — Bilimsel Danışma Raporu (önerilir, uygulanmaz)
- **B-01 (ACA-08 · betimleyici→eleştirel):** "pek iyi çalışmadığını" değerlendirme içerir ama `%12,4`
  dışında nicelleştirilmemiştir — bir hata oranını "iyi değil" yapan karşılaştırma/eşiği belirtmeyi
  değerlendirin.

### Yazar onayı
`consent_to_apply = verilmedi`.

### Sonuç — Kanal 3 ÜRETİLMEZ
Kanal 1 ve 2 tam olarak sunulur. **Kanal 3 yok; hiçbir danışma maddesi uygulanmadı; revizyon günlüğü
üretilmedi.** `%12,4` değişmedi. *(Bildirim: `ai_disclosure_policy=unknown` → yine de danışma niteliğinde
bir bildirim sunulur; sessizlik asla bir sonuç değildir.)*

> **Onay kapısı kanıtı:** düşünce düzeyindeki **B-01 uygulanmadı**; girdinin verisi bayt bayt korundu;
> **Kanal 3, beş koşulu sağlanmadığı için tutuldu** (onay verilmedi) — tam da kapı davranışı
> (Blueprint §11 G1).

---

*Skill reference — `tr` worked examples (parity with `before-after.md`), source-grounded [TR1][TR2][TR3].
© 2026 Dr. Aladdin Ali / Aladdin Pertanian Internasional.*
