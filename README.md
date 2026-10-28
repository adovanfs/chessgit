# Adovan — Landing Page Edukasi Catur

Landing page satu halaman, Bahasa Indonesia, tema gelap dengan aksen emas (#D4AF37).
Murni HTML, CSS, dan JavaScript (tanpa framework, tanpa proses build).

## Isi proyek
- `index.html`  : seluruh halaman (CSS dan JS sudah di dalam, diberi komentar per bagian)
- `.nojekyll`   : agar GitHub Pages menyajikan file apa adanya
- `README.md`   : panduan ini

## Fitur
Loader bertema catur, progress bar baca, navigasi sticky + daftar isi yang bisa dilipat,
mode gelap/terang, hero 3D dengan debu emas, timeline sejarah, esai filosofi,
papan mini interaktif tiap bidak (plus tur kuda dan delapan ratu), animasi aturan khusus,
taktik, lima pembukaan klasik, latihan "temukan langkahnya", kalkulator butir gandum,
garis waktu AI catur, FAQ, dan penutup.

## Deploy ke GitHub Pages
1. Buat repositori baru di GitHub (misalnya `adovan`).
2. Unggah `index.html`, `.nojekyll`, dan `README.md` ke cabang `main`.
3. Buka Settings > Pages > Source: pilih "Deploy from a branch", cabang `main`, folder `/ (root)`.
4. Tunggu satu sampai dua menit. Situs aktif di `https://<username>.github.io/adovan/`.
5. Domain kustom (opsional): isi kolom "Custom domain" di halaman Pages yang sama.

## Menyesuaikan
- Warna: ubah variabel di `:root` (awal bagian `<style>`), mis. `--gd` untuk emas.
- Teks: sebagian konten ada di array JavaScript (`T`, `P`, fakta, FAQ), sisanya langsung di HTML.
- Skenario animasi papan: lihat fungsi `demo(...)` dan daftar langkahnya.

## Catatan
- Font (Cormorant Garamond dan Hanken Grotesk) dimuat dari Google Fonts; tanpa internet, halaman memakai font cadangan.
- Animasi otomatis berhenti bila pengunjung mengaktifkan "kurangi gerakan" di perangkatnya.
- Latihan "temukan langkahnya" dan delapan ratu dioperasikan dengan klik/sentuh.
