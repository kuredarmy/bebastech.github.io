# Panduan Publish — Redesain BebasTech

Website sudah dirombak total dan siap tayang. File lengkap ada di `bebastech-redesign.zip`
(atau folder `bebastech-site/`), dan perubahan sudah di-commit di branch `main` secara lokal.

## Cara publish (pilih salah satu)

### Opsi A — Push langsung (paling cepat)
Jika akses GitHub `bebastech` sudah terhubung di perangkat ini:

```bash
cd ~/workspace/bebastech-site
git push origin main
```

GitHub Pages akan otomatis membangun ulang situs dalam 1–2 menit.
Cek status di: `https://github.com/kuredarmy/bebastech.github.io/actions`

### Opsi B — Upload manual via web GitHub
1. Buka `https://github.com/kuredarmy/bebastech.github.io`
2. Klik **Add file → Upload files**
3. Seret seluruh isi `bebastech-redesign.zip` yang sudah diekstrak
4. Commit langsung ke `main`

## Yang berubah dalam redesain ini

**Desain & pengalaman**
- Navigasi sticky dengan efek blur, menu hamburger di mobile, dropdown "Tentang"
- Hero dengan ilustrasi AI, statistik, dan tombol ajakan
- Kartu artikel dengan thumbnail, tag, tanggal Indonesia, dan estimasi waktu baca
- Halaman artikel: gambar hero, blok penulis, tombol share (X/WhatsApp/Telegram/salin tautan), artikel terkait
- Animasi scroll-reveal yang halus (nonaktif otomatis jika pengguna memilih reduced motion)
- Halaman 404 kustom yang ramah

**Bilingual (ID/EN)**
- Beranda Inggris hanya menampilkan artikel Inggris (bug campur bahasa diperbaiki)
- Halaman baru: `/en/about` dan `/en/contact` (sebelumnya link mati)
- Terjemahan Inggris artikel AI dilengkapi agar setara dengan versi Indonesia

**Bug yang diperbaiki**
- Favicon rusak (`/logo.png` 404) → logo baru sudah dipasang
- Kartu artikel duplikat di beranda → loop ganda dihapus
- Nama file postingan `026-...` → `2026-...` (tanggal valid)

**SEO & teknis**
- Meta description, Open Graph, Twitter Card, canonical URL, hreflang ID/EN
- `robots.txt` + `sitemap.xml`
- Favicon standar + Apple touch icon

## Yang perlu dicek setelah publish
- [ ] Buka `https://bebastech.web.id` — pastikan tampil versi baru (tunggu 1–2 menit setelah push)
- [ ] Cek `/en/`, `/about`, `/kontak`, `/en/about`, `/en/contact`
- [ ] Cek favicon di tab browser
- [ ] (Opsional) Daftarkan `sitemap.xml` di Google Search Console

## Catatan
- Link sosial sudah diperbarui 30 Sep 2026: LinkedIn `linkedin.com/in/kurniawan1314`, X `@kuredarmy`.
- Versi Inggris artikel "Era Baru Privasi dan Keamanan Digital" belum ada;
  beri tahu saya jika ingin dibuatkan.
