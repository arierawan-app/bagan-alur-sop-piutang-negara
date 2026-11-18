# Laporan Validasi Independen — Bagan Alur SOP Pengurusan Piutang Negara

Dua subagent validator memeriksa ulang seluruh klaim bagan secara **independen terhadap PDF asli** (read-only, tanpa internet/pengetahuan umum di luar dokumen). Hasil di bawah menjadi dasar koreksi pada `index.html`.

---

## Subagent 1 — Validasi klaim SOP (KEP-516/KN/2021, area `N-KPKNL-PN`, hlm. index-0 157–723)

Metode: ekstraksi teks per halaman (PyMuPDF) langsung dari PDF asli; batas SOP dipetakan ulang dari marker `N-KPKNL-PN` (98 kode ditemukan), tanpa bergantung pada hasil ekstraksi pihak lain.

### Ringkasan
| Kategori | Jumlah |
|---|---|
| Klaim SLA diperiksa | 65 |
| **SESUAI** | **64** |
| **TIDAK SESUAI** | **1** (SOP 32) |
| TIDAK DAPAT DIVERIFIKASI | 0 |
| Verifikasi tambahan | 7/7 terkonfirmasi |

### Ketidaksesuaian
- **SOP 32** — klaim "paling lama 6 hari kerja" → **TIDAK SESUAI**. Bukti (hlm. 330): *"7. Jangka Waktu Penyelesaian Paling lama 5 (lima) hari kerja"*. Koreksi telah diterapkan pada bagan (SOP 32 = ≤5 hk; SOP 34 = ≤6 hk, hlm. 339).

### Kutipan kunci terkonfirmasi
1. SOP 1 "11. Catatan Lainnya" (hlm. 160): definisi 1 hari kerja; pengecualian norma waktu (unit kerja lain; gangguan aplikasi >2 jam) dengan simbol penundaan (delay)/proses lain; kewenangan Plt./Plh. — **ketiga catatan khusus bagan verbatim**.
2. SOP 20 — anomali terkonfirmasi: judul & bagian 5/10 sesuai ("Surat Peringatan… keringanan"; pembayaran 7 hk bulanan / 30 hk triwulanan sejak tanggal surat peringatan), tetapi bagian 6 (Keluaran "Tanda Terima Dokumen Asli…"), 7 (SLA "Satu hari kerja"), 8 (Perhatian), 9 (RASCI) identik dengan SOP 21 — artefak duplikasi dokumen resmi.
3. SOP 14 — tiga pemicu PJPN verbatim (tidak mengakui & tak dapat membuktikan / mengakui tapi menolak tanda tangan PB tanpa alasan sah / tidak memenuhi panggilan & pengumuman).
4. SOP 9 — output: ND Laporan Ketersediaan Anggaran; pengumuman surat kabar/papan pengumuman; BA Penempelan Pengumuman.
5. SOP 61 = 8 hk (SPPB); SOP 69 = 2 hk + Deskripsi (hlm. 556): *"…diterbitkan oleh Panitia Cabang dalam jangka waktu paling lama 3 (tiga) hari sejak surat permohonan izin diterima"* → aturan "3 hari" melekat pada **izin keluar**, bukan penerbitan SPPB.
6. SOP 11 output = PB / ND pengantar PB; frasa "PB Tidak Sanggup" konteksnya di PMK 240 Psl 57–58 & SOP 52 (hlm. 451).
7. "4. Pihak-Pihak yang Terlibat": seluruh aktor terkonfirmasi ada, komposisi bervariasi per SOP — tidak ada satu SOP yang memuat semua aktor.

### Temuan tambahan
- **SOP urutan ke-65 tanpa nomor** (hlm. 535–539): "Penerbitan Surat Permintaan Bantuan Penyediaan Tempat Pelaksanaan Paksa Badan", kolom No. SOP **kosong**, SLA "enam hari kerja" — mengisi lacuna kode yang melompat 64→66; ditambahkan ke bagan.
- Typo sumber: "3 (tiga)) hari kerja" (SOP 92, 93); penomoran bagian 4 melompat (e→f) pada SOP 39/50/52/53/54.

---

## Subagent 2 — Validasi klaim regulasi (K1–K25)

Metode: grep seluruh dump teks + verifikasi langsung PDF asli (PP 28/2022, PP 4/2026, PMK 240/2016, PMK 23/2026, PMK 102/2017, KMK 144/2026 & Lampiran).

### Ringkasan
| Kategori | Jumlah |
|---|---|
| **SESUAI** | **23** (K1–K13, K16–K25) |
| **SEBAGIAN SESUAI** | **2** (K14, K15) |
| TIDAK SESUAI / TIDAK DITEMUKAN | 0 |

Seluruh nomor pasal pada klaim akurat. Dua koreksi: (1) regulasi memakai istilah penuh "Surat Perintah **Paksa Badan**" — singkatan "SPPB" hanya di dokumen SOP; (2) PMK 240 Psl 191 juga memuat syarat huruf d–e (PU mampu tapi tidak menunjukkan itikad baik; objek belum berumur 80 tahun).

### Konfirmasi kunci
- **Tarif BAPN 1% / 10% / 2,5% = NOL HIT** di seluruh PDF + PPTX folder → status *[Tidak diatur dalam dokumen sumber]*. BAPN diatur Psl 289–293: dikenakan sejak SP3N, proporsional, PNBP; besarnya merujuk peraturan lain.
- **Aturan "3 hari"** (Psl 214) = izin keluar Tempat Paksa Badan — bukan penerbitan SPPB.
- **PP 28/2022 Psl 52** verbatim (daftar PU/JU → pengangkatan jabatan pada badan publik; ayat 2: harus dipertimbangkan dalam setiap seleksi).
- **"STPPN" tidak ada** di sumber → SPnPPN; **"somasi"/"surat tagihan"/"KTP" 0 hit** → rincian dokumen penyerahan *[Tidak diatur dalam dokumen sumber]*.
- **PMK 23/2026**: Psl 1 diubah; **Psl 62–63 dihapus**; Bagian Kelima A Bab XV + Psl 186A–E disisipkan; Psl 233 (aset digital/kripto); Psl 294 + 297A–D (pembayaran: tunai/penyerahan aset/pengambilalihan); istilah Penanggung Utang.
- **PP 4/2026**: Psl 7 huruf a–ff (termasuk dd–ff: penguasaan fisik/penggunaan, pendayagunaan [huruf ee tak terbaca di scan — terkonfirmasi tidak langsung via 3 dokumen], pengambilalihan hak); Psl 26(6); Psl 32(2); Psl 66; Psl 78A.
- **PMK 102/2017**: Ketua/Sekretaris PUPN Pusat = Dirjen/Direktur (Psl 5); Ketua PUPN Cabang = Kepala Kanwil (Psl 7); anggota Kemenkeu = Kepala KPKNL (Psl 8); Sekretariat (Psl 22–24); Ketua PUPN Cabang dapat menetapkan sendiri Nilai Limit/Penebusan/Penjualan Tanpa Lelang (Psl 10).
- **PP 28/2022 Psl 69 huruf b** juga mencakup PU "bermasalah yang sulit diselesaikan"; syarat moneter: PSBDT pemeriksaan ≥ Rp500 jt (Psl 282), penelitian lapangan ≤ Rp50 jt (Psl 283), pengecualian ≤ Rp25 jt & >10 th (Psl 284), ≤ Rp8 jt + KKM/asuransi (Psl 285), tunai di KPKNL maks Rp50 jt (Psl 295).
- **PMK 240 Psl 307**: ≤14 hari BAPN penarikan → teguran → Surat Pembatalan Persetujuan Penarikan (ayat 2).
- **Kronologi konsisten**: PP 4/2026 (26 Jan 2026) → PMK 23/2026 (21 Apr 2026) → KMK 144/2026 (29 Apr 2026); PMK 23/2026 merujuk PP 4/2026 pada Pasal 66.
- **Keterbatasan**: KMK 724/2017 & KMK 182/2022 scan tanpa lapisan teks — tidak ada klaim yang merujuk langsung isinya; format lama (angka 1–41) terverifikasi tidak langsung.

### Catatan editorial dokumen sumber
- PMK 240 Psl 266(3) salah rujukan silang ("ayat (1)" — logisnya ayat (2)).
- PMK 23/2026 Psl 186E(1) typo penomoran ("b." ganda); frasa "paling singkat 10 hari kerja" (Psl 186B/186D/297C) tidak lazim.
- Salinan PP 28/2022 & PP 4/2026 ber-OCR dengan artefak (mis. "SPSN" untuk SP3N) — substansi tidak terpengaruh.

---

## Koreksi yang telah diterapkan pada bagan

1. Node `32/34-KPKNL-PN`: SLA dipisah — SOP 32 ≤5 hk, SOP 34 ≤6 hk.
2. Node baru `SOP tanpa nomor (urutan ke-65)` — Minta Bantuan Penyediaan Tempat Pelaksanaan Paksa Badan (6 hk), tersambung ke lane Lapas/Rutan.
3. Node `59-KPKNL-PN`: syarat dilengkapi Psl 191 huruf d–e.
4. Node `92-KPKNL-PN`: kondisi "bermasalah yang sulit diselesaikan" + ambang Rp500 jt/Rp50 jt.
5. Node `93-KPKNL-PN`: teguran → Surat Pembatalan Persetujuan Penarikan.
6. Bagian "Temuan Validasi" pada `index.html` memuat tabel koreksi klaim prompt di atas.
