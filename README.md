# Bagan Alur End-to-End SOP Pengurusan Piutang Negara oleh PUPN (KPKNL)

Halaman interaktif berisi **satu bagan alur (flowchart) end-to-end** Standar Operasional
Prosedur Pengurusan Piutang Negara oleh PUPN pada KPKNL — disusun **100% dari dokumen
sumber** pada folder `PERATURAN` (KPKNL Kupang), tanpa sumber eksternal.

> 🌐 **Halaman utama (GitHub Pages):** https://arierawan-app.github.io/bagan-alur-sop-piutang-negara/

## Isi halaman

1. **Bagan alur Mermaid — alur kronologis ringkas** (35 simpul): satu alur utama dengan 6 titik keputusan — hasil penelitian kasus (SP3N/kelengkapan/penolakan), PU hadir & sepakat, wanprestasi PB, lunasi 1×24 jam, syarat Paksa Badan, dan hasil lelang. Simpul memuat **No. SOP + SLA**; dokumen kunci mengalir sebagai label garis; aktor penting tercantum inline (Kepala KPKNL, Ketua PUPN Pusat/Cabang, Menteri, Juru Sita, Kepala Kejaksaan Tinggi, Lapas/Rutan).
   - Empat tahap: T1 Penerimaan & Penanganan Barjam · T2 Pemanggilan & Produk Hukum Awal · T3 Pemeriksaan, Paksa & Sita · T4 Keringanan, Penebusan & Penyelesaian Akhir.
   - **Arsip versi rinci per aktor** (swimlane, 95 simpul): [`bagan_sop_piutang_negara.mmd`](bagan_sop_piutang_negara.mmd) — sumber bagan utama ringkas: [`bagan_alur.mmd`](bagan_alur.mmd).
2. **Ketentuan khusus** — definisi 1 hari kerja, simbol penundaan (delay)/proses lain, kewenangan Plt./Plh. (Catatan Lainnya tiap SOP).
3. **Kondisi terkini 2026** — ringkasan PMK 23/2026, PP 4/2026, KMK 144/2026.
4. **Temuan validasi** — koreksi atas klaim prompt, divalidasi independen oleh 2 subagent terhadap PDF asli.
5. **Tabel traceability** — setiap klaim simpul → halaman KEP-516/KN/2021 dan pasal PP/PMK/KMK.

## Konvensi simbol (BPMN DJKN)

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
