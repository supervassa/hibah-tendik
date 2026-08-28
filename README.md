# Aplikasi Digital PPKS — Universitas Jember

Recovery & penyelesaian **Hibah Penelitian Tenaga Kependidikan Universitas Jember Tahun 2026**.

**Judul penelitian:** Pengembangan Aplikasi Digital Pencegahan dan Penanganan Kekerasan Seksual (PPKS) di Universitas Jember
**Ketua peneliti:** Juris Vassa Ivandro, S.Kom. — UPA TIK Universitas Jember (PPPK, Programmer)
**Skema hibah:** Hibah Penelitian Tenaga Fungsional Non Dosen
**Dana:** Rp5.000.000
**Rencana pelaksanaan awal (proposal):** April–Juni 2026

## Ringkasan

Proyek ini mengembangkan aplikasi pelaporan dan penanganan kasus PPKS di Universitas Jember, dengan dua sisi pengguna: **Pelapor** (publik, tanpa login) dan **Satgas** (login, pengelolaan kasus). Pendekatan teknologi disederhanakan dari rencana awal (Web Dashboard React+Node terpisah dari Mobile App Flutter) menjadi satu platform **Progressive Web Application (PWA)** agar dapat dipakai di desktop maupun mobile dengan satu codebase, sesuai jawaban atas komentar reviewer.

Metodologi penelitian mengacu pada **ADDIE** (Analysis → Design → Development → Implementation → Evaluation).

## Status saat ini (per 28 Agustus 2026)

Proposal diajukan Februari 2026, namun penelitian terlambat dimulai. Pendekatan yang dipakai adalah **recovery plan**, bukan laporan seolah-olah seluruh tahapan sudah selesai. Rincian status:

**Sudah ada / selesai:**
- Draft revisi proposal (`docs/prposal/Proposal Revisi - Hibah PPKS UNEJ 2026.docx`) menjawab komentar Reviewer 1 (template & kontribusi lembaga/IKU/WCU) dan Reviewer 2 (inovasi & keberlanjutan jangka panjang), termasuk perubahan pendekatan teknologi ke PWA.

**Sedang dikerjakan:**
- Penyusunan struktur dokumentasi recovery (folder `app/`, `database/`, `prototype/`, `docs/`) di repo ini.

**Belum dikerjakan:**
- Analisis kebutuhan & desain sistem (skema database, spesifikasi API).
- Pengembangan prototype aplikasi (frontend React/Tailwind, backend Node.js/REST API, database PostgreSQL).
- UAT, security testing, usability testing.
- Laporan kemajuan (draft ada di `docs/laporan-kemajuan/`, belum disusun isinya).
- Materi presentasi Monev maksimal 10 menit (folder `docs/monev/`, belum disusun).

**Rencana tindak lanjut:**
- Menyusun MVP dengan alur inti: Pelapor membuat laporan simulasi → mendapat kode laporan → Satgas melihat & mengubah status laporan → Pelapor mengecek status, menggunakan data simulasi/dummy saja (bukan data korban/kasus nyata).

> Catatan: seluruh proses pengembangan dan demonstrasi aplikasi menggunakan **data simulasi/dummy**. Tidak ada data korban atau kasus nyata yang digunakan atau disimpan dalam repo ini. Tidak ada klaim hasil pengujian, capaian, atau dokumentasi kegiatan yang dituliskan tanpa bukti nyata.

## Rencana fitur aplikasi

**Sisi Pelapor (publik):**
informasi PPKS, formulir pelaporan, kategori laporan, kronologi, upload bukti, kode laporan, cek status laporan.

**Sisi Satgas (login):**
dashboard, daftar laporan, detail laporan, update status, penugasan, riwayat penanganan, statistik, laporan periodik.

## Rencana teknologi

| Komponen | Teknologi |
|---|---|
| Application type | Progressive Web Application (PWA) |
| Frontend | React.js |
| UI Framework | Tailwind CSS |
| Backend | Node.js |
| API | REST API |
| Database | PostgreSQL |
| Version control | Git |

## Struktur repo

```
.
├── app/                  # Kode aplikasi (frontend + backend) — belum ada implementasi
├── database/             # Skema & migrasi PostgreSQL — belum ada implementasi
├── prototype/            # Prototype/MVP PWA — belum ada implementasi
├── docs/
│   ├── prposal/          # Draft revisi proposal hibah
│   ├── reviewer/         # Catatan/komentar reviewer & tindak lanjut
│   ├── laporan-kemajuan/ # Draft laporan kemajuan
│   └── monev/            # Materi presentasi Monev
├── Instruksi_Recovery_Hibah_PPKS_2026.md   # Instruksi lengkap tahapan recovery
└── proposal hibah tendik juris.pdf         # Proposal awal (Februari 2026)
```

## Menjalankan aplikasi

Belum tersedia — prototype belum dikembangkan. Bagian ini akan diisi setelah tahap Development (ADDIE) menghasilkan MVP yang bisa dijalankan.

## Referensi internal

- `Instruksi_Recovery_Hibah_PPKS_2026.md` — instruksi lengkap tahap recovery: audit kondisi, revisi proposal, analisis kebutuhan, desain sistem, development, testing, dokumentasi, laporan kemajuan, hingga PPT Monev.
