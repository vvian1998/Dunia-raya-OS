# CHANGELOG — Dunia Raya OS v8.4

## v8.4 — UX Polish & Dashboard Alive Update

### Added
- Dynamic greeting berdasarkan waktu: pagi, siang, sore, malam.
- Quote harian random dengan minimal 8 variasi per waktu.
- Section **Insight Hari Ini** di Home.
- Wealth summary: Total Pockets, Total Assets, Total Target, Overall Progress.
- Premium empty state untuk Journal, Assets, Transaksi, Learning Log, dan Goals.
- Contextual Floating Action Button.
- Quick Add Menu: Catat Transaksi, Tulis Journal, Tambah Goal, Tambah Asset.
- Modal konfirmasi untuk Clear Data, Factory Reset, dan Reset PIN.
- Input konfirmasi `RESET` untuk Factory Reset.
- PIN screen premium dengan keypad 3x4, show/hide PIN, feedback error, shake animation, success animation, dan dukungan keyboard fisik.
- Export JSON kini membawa metadata `version: 8.4`, events, profile, dan theme.

### Improved
- Dark mode dibuat lebih premium dengan charcoal/navy gelap, card slate, border soft, text lembut, dan gold accent.
- Progress bar dibuat lebih tebal dan animasi smooth dari 0 ke nilai target.
- Micro-interactions untuk button, card, modal, tab/screen, dan FAB.
- Profile polish: nama, role/profession, badge, avatar, initial fallback, dan localStorage.
- Empty state sekarang lebih hangat, informatif, dan punya CTA.
- Wealth dashboard tidak lagi terasa seperti spreadsheet.
- Home terasa lebih seperti command center.

### Safety
- Tidak merombak struktur utama aplikasi.
- Data existing tetap memakai localStorage key lama.
- Clear Data menjaga PIN tetap tersimpan.
- Factory Reset membersihkan key DROS/user secara menyeluruh.
- Single-file PWA tetap bisa dibuka langsung dari `index.html`.

## v8.6 — Finance UI Patch (Wealth Transaction Polish)

### Added
- Finance overview di halaman Wealth: Net Worth Tercatat, Masuk Bulan Ini, Keluar Bulan Ini, Sisa Cashflow, dan Total Assets.
- Card transaksi baru yang lebih bersih dengan ikon kategori, judul transaksi berbasis catatan, meta kategori + tanggal manusiawi, dan nominal besar.
- Menu aksi transaksi via tombol `⋮` berisi Edit, Duplikat, dan Hapus.
- Helper kategori emoji untuk Makan, Transport, Tagihan, Rumah, Pendidikan, Keluarga, Hiburan, Gaji, dan default.

### Improved
- Tombol Edit/Hapus tidak lagi selalu tampil di card transaksi sehingga UI lebih premium dan tidak terasa seperti CRUD.
- FAB tidak lagi menutupi konten terakhir karena screen diberi padding bawah lebih lega.
- Warna income/expense dibuat lebih lembut dan premium.
- Tanggal transaksi tampil lebih manusiawi seperti Hari ini, Kemarin, atau format tanggal Indonesia.


## v8.4.1 — Wealth UI Refinement

### Improved
- Halaman Wealth tab Transaksi dibuat lebih ringkas dan tidak crowded.
- Statistik utama dipadatkan menjadi Net Worth, Masuk, Keluar, Cashflow, dan Progress.
- Total Pockets, Total Assets ganda, dan Total Target tidak lagi memenuhi tab Transaksi.
- Card transaksi dibuat lebih bersih dengan ikon kategori, judul berbasis deskripsi, tanggal manusiawi, dan nominal yang jelas.
- Tombol Edit/Hapus langsung diganti menjadi menu `⋮` agar UI lebih tenang.
- Ditambahkan insight cashflow singkat agar Wealth terasa lebih hidup.
- FAB spacing diperbaiki agar tidak menutupi card terakhir.

### Notes
- Patch ini mempertahankan struktur v8.4 dan tidak mengubah data localStorage.
- Fokus patch adalah efisiensi visual dan kenyamanan pemakaian harian.

## v8.4.2 — Finance Input UX Polish

### Improved
- Input nominal transaksi sekarang otomatis memformat angka ribuan. Contoh: `3000` langsung tampil sebagai `3.000`.
- Form transaksi dibuat lebih cepat dan lebih nyaman dibaca: tipe, nominal, kategori, catatan, lalu simpan.
- Kategori transaksi tidak lagi wajib diketik manual. Pengguna dapat memilih dari kategori siap pakai seperti Makan, Jajan, Transport, Tagihan, Keluarga, Gaji, Belanja, Kesehatan, Pendidikan, Hiburan, dan Lainnya.
- Opsi Custom tetap tersedia untuk kategori khusus.
- Ikon transaksi diganti dari emoji menjadi SVG line icon agar lebih konsisten, premium, dan tidak bergantung pada rendering emoji Android.
- Konfirmasi hapus transaksi diganti dari popup Android/Browser default menjadi bottom sheet bergaya DROS.

### Notes
- Patch ini fokus pada pengalaman input finance harian agar pencatatan transaksi terasa lebih cepat, rapi, dan tidak seperti form teknis.
