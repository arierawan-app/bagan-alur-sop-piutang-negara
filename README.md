# Bagan Alur End-to-End SOP Pengurusan Piutang Negara oleh PUPN (KPKNL)

Halaman interaktif berisi **satu bagan alur (flowchart) end-to-end** Standar Operasional
Prosedur Pengurusan Piutang Negara oleh PUPN pada KPKNL — disusun **100% dari dokumen
sumber** pada folder `PERATURAN` (KPKNL Kupang), tanpa sumber eksternal.

> 🌐 **Halaman utama (GitHub Pages):** https://arierawan-app.github.io/bagan-alur-sop-piutang-negara/

## Isi halaman

1. **Alur Prosedur Interaktif (HTML dinamis — tanpa bagan)** — 73 kartu SOP yang dapat dicari & dibuka/tutup, terbagi 4 tahap + Status Akhir:
   - Tiap kartu SOP memuat: **persyaratan (dokumen masukan)** verbatim, **referensi peraturan** (pasal PP/PMK/KMK), **keluaran (produk/dokumen)**, **jangka waktu penyelesaian** ditulis penuh (mis. "paling lama enam (6) hari kerja" — tanpa singkatan), **dasar hukum** (bagian 2 SOP), dan **pihak yang terlibat**.
   - 6 **kartu keputusan** (hasil penelitian, hadir & sepakat, wanprestasi PB, lunas 1×24 jam, syarat Paksa Badan, hasil lelang) dengan tautan lompat langsung ke SOP tujuan.
   - Fitur: tab per tahap, pencarian langsung lintas tahap (nomor SOP / dokumen / kata kunci), buka-tutup semua, pita alur utama yang dapat diklik.
   - **Arsip versi bagan (Mermaid)**: [`bagan_alur.mmd`](bagan_alur.mmd) (alur kronologis ringkas) dan [`bagan_sop_piutang_negara.mmd`](bagan_sop_piutang_negara.mmd) (rinci per aktor/swimlane).
2. **Ketentuan khusus** — definisi 1 hari kerja, simbol penundaan (delay)/proses lain, kewenangan Plt./Plh. (Catatan Lainnya tiap SOP).
3. **Kondisi terkini 2026** — ringkasan PMK 23/2026, PP 4/2026, KMK 144/2026.
4. **Temuan validasi** — koreksi atas klaim prompt, divalidasi independen oleh 2 subagent terhadap PDF asli.
5. **Tabel traceability** — setiap klaim simpul → halaman KEP-516/KN/2021 dan pasal PP/PMK/KMK.

## Konvensi simbol (berlaku untuk arsip bagan Mermaid — BPMN DJKN)

| Simbol | Arti |
|---|---|
| ─── | alur proses internal (garis tegas) |
| ┄┄┄ | aliran dokumen / interaksi antar pihak (garis putus-putus) |
| `{ }` | percabangan keputusan (gateway X) |
| ⏸ | simpul penundaan/proses lain — norma waktu dikecualikan |
| 🏁 | status akhir (SPPNL, SPPNS, SKPPN, PSBDT, SPnPPN, PTDM) |

## Sumber (semua dari folder PERATURAN)

- **KEP-516/KN/2021** — Perubahan Keempat SOP KPKNL (SOP `1`–`99-KPKNL-PN`, hlm. area Piutang Negara)
- **PP 28/2022** jo. **PP 4/2026** — Pengurusan Piutang Negara oleh PUPN
- **PMK 240/PMK.06/2016** jo. **PMK 23/PMK.06/2026** — Pengurusan Piutang Negara
- **PMK 102/PMK.06/2017** — Keanggotaan dan Tata Kerja PUPN
- **KMK 724/KM.6/2017** jo. **KMK 182/KM.6/2022** jo. **KMK 144/MK/KN/2026** — Format Naskah Dinas & Produk Hukum PUPN
- **PER-06/KN/2017** & **PER-04/KN/2009** — sebagaimana dicantumkan dalam dasar hukum SOP (dokumen tidak tersedia di folder)

Detail yang tidak tertulis eksplisit pada dokumen sumber ditandai
**[Tidak diatur dalam dokumen sumber]** — tidak diarang.

---

_Disusun otomatis dari dokumen sumber; divalidasi silang independen oleh 2 subagent
terhadap PDF asli. Mermaid.js di-render sisi klien via CDN._
