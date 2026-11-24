# Berita Kripto Harian

Situs berita crypto berbahasa Indonesia, diperbarui setiap hari.
Live di Netlify (alamat menyusul setelah deploy).

## Cara kerja

- `index.html` — halaman utama; mengambil daftar berita dari `news.json` dan harga
  live dari API publik CoinGecko (tanpa kunci API).
- `news.json` — data berita harian (judul, ringkasan Bahasa Indonesia, sumber + tautan,
  snapshot harga, dan indeks Fear & Greed). Diperbarui setiap pagi oleh cron harian.
- `tentang.html`, `privasi.html`, `kontak.html` — halaman pendukung (syarat AdSense).

## Update harian

Setiap pagi (~07:00 WIB) berita terbaru diambil dari sumber terpercaya (CoinDesk,
CoinStats, TradingView, FXStreet, dan sejenisnya), dirangkum dalam Bahasa Indonesia,
lalu `news.json` diperbarui dan Netlify men-deploy ulang otomatis dari repo ini.

Konten hanya informasi, bukan nasihat investasi.
