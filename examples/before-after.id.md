<!--
Copyright (c) 2026 Dr. Aladdin Ali - Founder of Aladdin Pertanian Internasional - dr.alaa@aladdin.my.id. All Rights Reserved.
-->

# Contoh Terkerjakan (Bahasa Indonesia) — Worked Examples (Indonesian)
## Skill reference — `id` SOURCE-GROUNDED ([ID1] UGM · [ID2] Panduan Makalah Ilmiah · [ID3] UPI)
### Setara penuh dengan berkas Inggris `before-after.md` / at full parity with the English file

> Contoh ini **setara kedalamannya** dengan `before-after.md` (Inggris): tiga kanal, **dua butir saran**
> (A-01 + A-02), **log revisi** lengkap, dan **gerbang persetujuan** — dalam Bahasa Indonesia. Setiap
> angka/kutipan/DOI **dipertahankan persis** (INV-A1). Kaidah Indonesia bersumber diterapkan: kalimat ditulis
> dalam **bentuk pasif tanpa sudut pandang orang pertama/kedua** (*saya/kami/Anda*) [ID1 §3.4.2]. Model tiga
> kanal dan gerbang persetujuan **identik** dengan versi Inggris.

---

## Contoh 1 — Klaim berlebihan + de-AI, alur penuh (persetujuan diberikan)

**Kontrak:** `level=journal` · `programme_type=journal` · `edit_scope=apply_approved_notes` ·
`co_authored=false` · `ai_disclosure_policy=required` · `output_language=id`.

**Masukan (paragraf pembahasan):**
> "Sebagai kesimpulan, penelitian terobosan kami secara jelas membuktikan bahwa Obat X menyebabkan
> pendarahan! 😊 Penelitian menunjukkan bahwa ini adalah temuan yang penting. Dalam percobaan kami, kami
> mengamati pendarahan pada **18** dari **20** pasien (lihat **Tabel 2**), yang konsisten dengan Almeida dkk.
> **[7]**."

### Kanal 1 — Teks yang Diperbaiki Bahasanya (otomatis, hanya ungkapan)
> "Penelitian ini secara jelas membuktikan bahwa Obat X menyebabkan pendarahan. Penelitian menunjukkan bahwa
> ini adalah temuan yang penting. Dalam percobaan ini, pendarahan diamati pada **18** dari **20** pasien
> (lihat **Tabel 2**), yang konsisten dengan Almeida dkk. **[7]**."

*Diubah (hanya ungkapan):* "Sebagai kesimpulan," dihapus (HUM-25); "terobosan" dihapus (HUM-01); "! 😊"
dihapus (HUM-18). **Kaidah persona/diatesis (ACA-04 · [ID1] §3.4.2):** "penelitian … kami" → "penelitian
ini"; orang pertama *"Dalam percobaan kami, kami mengamati"* → **pasif** *"Dalam percobaan ini, … diamati"*.
*Dipertahankan:* klaim **"secara jelas membuktikan … menyebabkan"** (kekuatan klaim — Kanal 2, ACA-01);
ungkapan tanpa rujukan **"Penelitian menunjukkan"** (HUM-05, dalam mode akademik → Kanal 2); dan
**`18` · `20` · `Tabel 2` · `[7]`** — persis (INV-A1).

### Kanal 2 — Laporan Saran Ilmiah (disarankan, tidak diterapkan)
- **A-01 (ACA-01 · klaim berlebihan/objektivitas):** "secara jelas membuktikan bahwa Obat X menyebabkan
  pendarahan" melampaui satu percobaan (18/20) dan melanggar prinsip **objektif** [ID2]/[ID3]. Saran yang
  terbatas pada sampel dan berhati-hati: *"Pada sampel ini, pendarahan diamati pada sebagian besar pasien,
  yang dapat mengindikasikan masalah keamanan yang memerlukan penelitian lebih lanjut."* *(mengubah kekuatan
  klaim — keputusan penulis)*
- **A-02 (HUM-05 / ACA-02 · rujukan kabur):** "Penelitian menunjukkan bahwa ini adalah temuan yang penting"
  tanpa rujukan — kutip penelitian spesifik, batasi, atau hapus. *(jangan pernah mengarang rujukan — AIP-3)*

### Persetujuan penulis
`consent_to_apply = diberikan`, diterima: **A-01, A-02** (penulis memilih **menghapus** kalimat tanpa
rujukan); `authorship_acknowledgement = dikonfirmasi`.

### Kanal 3 — Revisi Ilmiah yang Disetujui Penulis (diterapkan + dimanusiakan)
> "Penelitian ini mengkaji hubungan antara Obat X dan pendarahan. Dalam percobaan ini, pendarahan diamati
> pada **18** dari **20** pasien (lihat **Tabel 2**), yang dapat mengindikasikan masalah keamanan yang
> memerlukan penelitian lebih lanjut, dan konsisten dengan Almeida dkk. **[7]**."

### Log revisi (INV-A10)
**Kepala:** `id` · `journal`/`journal` · `apply_approved_notes` · `co_authored=false` ·
`ai_disclosure_policy=required` → pernyataan penggunaan AI disertakan · diterima: `A-01, A-02` ·
`authorship_acknowledgement=dikonfirmasi`.

| change_id | lokasi | kanal | butir disetujui | sebelum → sesudah | alasan | pemeriksaan invarian |
|-----------|--------|:-----:|-----------------|-------------------|--------|----------------------|
| C-001 | Pembahasan ¶ | K.3 | A-01 | "secara jelas membuktikan … menyebabkan pendarahan … pendarahan diamati pada 18 dari 20 → Penelitian ini mengkaji hubungan antara Obat X dan pendarahan … dapat mengindikasikan masalah keamanan …" | penulis menerima ungkapan terbatas-sampel (klaim kausal berlebihan dihapus) | INV-A6: klaim dipersempit atas persetujuan penulis; angka tidak berubah |
| C-002 | Pembahasan ¶ | K.3 | A-02 | "Penelitian menunjukkan bahwa ini adalah temuan yang penting. → *(dihapus)*" | penulis menyetujui penghapusan rujukan kabur | INV-A2/A3: tidak ada yang dikarang; dihapus oleh penulis |
| C-003 | Pembahasan ¶ | K.1 | — (ACA-04 · [ID1] §3.4.2) | "Dalam percobaan kami, kami mengamati → Dalam percobaan ini, … diamati" | kaidah pasif tanpa orang pertama (otomatis, makna terjaga) | INV-A6: makna terjaga |
| C-004 | Pembahasan ¶ | K.1 | — (HUM-01/18/25) | "Sebagai kesimpulan, penelitian terobosan kami … ! 😊 → Penelitian ini …" | de-AI tingkat ungkapan saja | INV-A6: makna terjaga |

**Kesetiaan & pernyataan:** `18` → tidak berubah · `20` → tidak berubah · `Tabel 2` → tidak berubah ·
`[7]` → tidak berubah. Tidak ada batasan ilmiah yang dihapus; bukti lemah tidak diubah menjadi klaim kuat
tanpa butir yang disetujui. Pernyataan: pernyataan penggunaan AI disertakan; tanpa klaim "tak terdeteksi".
**Tanggung jawab penelitian utama tetap pada penulis**, dan kewenangan akhir pada pembimbing serta panitia
sidang.

---

## Contoh 2 — Gerbang persetujuan (persetujuan **tidak diberikan** → tanpa Kanal 3)

**Kontrak:** `level=masters` · `programme_type=masters_thesis` · `edit_scope=language_clarity` ·
`co_authored=false` · `ai_disclosure_policy=unknown` · `output_language=id`.

**Masukan:**
> "Anda dapat dengan jelas melihat pada **Gambar 3** bahwa model sebenarnya tidak bekerja dengan baik, yang
> merupakan keterbatasan penting. Tingkat kesalahannya adalah **12,4%**."

### Kanal 1 — Teks yang Diperbaiki Bahasanya (otomatis, hanya ungkapan)
> "**Gambar 3** menunjukkan bahwa model sebenarnya tidak bekerja dengan baik, yang merupakan keterbatasan
> penting. Tingkat kesalahannya adalah **12,4%**."

*Diubah (hanya ungkapan):* orang kedua "Anda dapat … melihat pada Gambar 3" → bentuk takpersona "Gambar 3
menunjukkan" (ACA-04 · [ID1] §3.4.2). *Dipertahankan:* pelembut "sebenarnya" (menghapusnya memperkuat klaim
→ Kanal 2); dan **`12,4%`** — persis, format desimal koma Indonesia **tidak diubah** (INV-A1).

### Kanal 2 — Laporan Saran Ilmiah (disarankan)
- **B-01 (ACA-08 · deskriptif→kritis):** "tidak bekerja dengan baik" bersifat evaluatif tetapi tidak
  terkuantifikasi selain 12,4% — sebutkan perbandingan/ambang yang membuat tingkat ini "tidak baik".

### Persetujuan penulis
`consent_to_apply = tidak diberikan`.

### Hasil — Kanal 3 tidak diproduksi
Kanal 1 dan 2 diserahkan lengkap. **Tidak ada Kanal 3; tidak ada butir saran yang diterapkan; tidak ada log
revisi yang diproduksi.** `12,4%` tidak berubah. *(Pernyataan: `ai_disclosure_policy=unknown` → pernyataan
saran tetap diberikan; kebisuan tidak pernah menjadi hasil.)*

> **Bukti gerbang persetujuan:** butir tingkat-pemikiran **B-01 tidak diterapkan**; data masukan dipertahankan
> persis; **Kanal 3 ditahan** karena lima syaratnya tidak terpenuhi (persetujuan tidak diberikan) — tepat
> perilaku gerbang (Blueprint §11 G1).

---

*Skill reference — `id` worked examples (full parity with `before-after.md`: A-01+A-02, 4-row revision log),
source-grounded [ID1][ID2][ID3]. © 2026 Dr. Aladdin Ali / Aladdin Pertanian Internasional.*
