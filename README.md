# Dunia Raya OS

**Dunia Raya OS** adalah Personal Operating System berbasis single-file PWA/HTML untuk mengelola ruang hidup pribadi: wealth, goals, journal, profile, dan insight harian.

Versi aktif: **v8.4 — UX Polish & Dashboard Alive Update**

## Identitas

- Nama: Dunia Raya OS
- Konsep: Personal Operating System
- Warna utama: navy / biru gelap
- Aksen: gold
- Navigasi utama: Home, Wealth, Goals, Journal, More
- Format aplikasi: mobile-first PWA, tetap bisa dibuka langsung dari `index.html`

## Isi Release

```text
DuniaRayaOS/
├── index.html
├── CHANGELOG.md
├── README.md
├── manifest.json
└── sw.js
```

Catatan: `manifest.json` dan `sw.js` dipertahankan sebagai file pendukung PWA. Aplikasi utama tetap berada di `index.html`.

## Highlight v8.4

- Dynamic greeting berdasarkan waktu: pagi, siang, sore, malam.
- Quote random agar sapaan tidak monoton.
- Home memiliki section **Insight Hari Ini**.
- Premium empty state untuk journal, assets, transaksi, learning log, dan goals.
- PIN screen lebih premium dengan keypad, show/hide PIN, feedback error, animasi, dan dukungan keyboard fisik.
- Progress bar lebih hidup dengan smooth animation.
- Wealth dashboard memiliki summary atas: Total Pockets, Total Assets, Total Target, Overall Progress.
- Destructive action memakai modal konfirmasi.
- Factory reset membutuhkan input `RESET`.
- Dark mode lebih premium dengan charcoal/navy gelap, card slate, dan gold accent.
- FAB kontekstual sesuai tab.
- Profile polish: nama, role, badge, avatar/fallback initial, tersimpan ke localStorage.
- Export/import disesuaikan agar membaca data baru dan tetap toleran terhadap data lama.

## Cara Deploy

### Netlify / Static Hosting

Upload isi folder ini ke Netlify, GitHub Pages, Vercel static, atau hosting statis lain.

Entry point:

```text
index.html
```

### Buka Langsung

`index.html` tetap bisa dibuka langsung di browser tanpa build step.

## Data Safety

DROS memakai `localStorage` di perangkat pengguna. Sebelum melakukan import, clear data, atau factory reset, lakukan export backup JSON terlebih dahulu.

## Roadmap Ringkas

### v8.5 — Data Depth & Daily Review

- Daily review ringan di Home.
- Filter transaksi bulanan.
- Journal mood/tag sederhana.
- Learning log timeline.
- Insight finansial lebih kaya.

### v8.6 — Backup & Restore Hardening

- Validasi backup sebelum import.
- Preview isi backup sebelum overwrite.
- Backup terenkripsi opsional.
- Restore selective.

### v8.7 — Offline PWA Polish

- Cache service worker lebih kuat.
- Offline fallback.
- Install prompt custom.
- Icon dan splash screen final.

### v9.0 — DROS Intelligence Layer

- AI insight lokal berbasis rule engine.
- Skor finansial personal.
- Skor konsistensi goals.
- Weekly review otomatis.

## Prinsip Pengembangan

- Jangan merombak total struktur aplikasi.
- Jangan menghapus fitur lama tanpa alasan kuat.
- Mobile-first.
- Aman terhadap localStorage existing.
- UI harus terasa personal, tenang, premium, dan manusiawi.
