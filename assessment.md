# Assessment — DROS v8.4.2 Finance Input UX Polish

Patch v8.4.2 berfokus pada pengalaman input transaksi harian. Area yang diperbaiki adalah bagian yang paling sering dipakai pengguna: memasukkan nominal, memilih kategori, dan mengelola transaksi.

## Hasil Perbaikan

- Nominal sekarang lebih mudah dibaca karena otomatis memakai format ribuan. Pengguna yang mengetik `3000` akan melihat `3.000` tanpa perlu memproses angka mentah.
- Kategori tidak lagi manual penuh. Pengguna bisa memilih kategori siap pakai seperti Makan, Jajan, Transport, Tagihan, Keluarga, Gaji, Belanja, Kesehatan, Pendidikan, Hiburan, dan Lainnya.
- Opsi Custom tetap disediakan agar aplikasi tidak terasa kaku.
- Ikon transaksi memakai SVG line icon sehingga lebih konsisten dengan identitas DROS yang premium dan tidak bergantung pada emoji Android.
- Hapus transaksi tidak lagi memakai popup bawaan browser/Android, tetapi memakai bottom sheet konfirmasi khas DROS.

## Dampak UX

Sebelum patch, form transaksi masih terasa seperti input teknis: nominal mentah, kategori diketik manual, dan beberapa aksi memakai popup bawaan sistem. Setelah patch, alurnya lebih terasa seperti aplikasi yang matang: pilih tipe, masukkan nominal, pilih kategori, tambah catatan, simpan.

## Catatan Lanjutan

Masih ada beberapa popup sistem pada modul lain seperti import backup, delete goal, delete journal, delete asset, dan event/reminder. Patch ini sengaja difokuskan dulu pada transaksi karena transaksi adalah alur paling sering dipakai dalam pencatatan keuangan.
