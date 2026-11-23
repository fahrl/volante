# Volante

Aplikasi web analisis gaya bermain klub (FotMob, 5 liga top Eropa, 2021/22–2025/26).
Dibuat oleh Fahri Syaifullah. Situs statis: tidak butuh backend.

## Isi folder
- `index.html` : kerangka halaman
- `style.css`  : tampilan
- `app.js`     : grafik dan logika
- `data.json`  : seluruh data, hasil sel ekspor notebook (`app_data.json`)

## Melihat di komputer
Aplikasi memuat `data.json`, jadi tidak bisa dibuka dengan klik dua kali.
Di folder ini jalankan:

    python -m http.server 8000

lalu buka http://localhost:8000

## Memperbarui data
1. Jalankan ulang notebook: sel ekspor, lalu sel final.
2. Unduh `app_data.json`.
3. Ganti isi `data.json` dengan file itu (ganti nama menjadi `data.json`).
Struktur kuncinya harus sama. Kalau notebook mengubah kunci atau urutan dimensi, `app.js` perlu disesuaikan.

## Hosting (GitHub Pages)
1. Buat repositori publik di GitHub, unggah keempat file di atas ke akar repositori.
2. Settings > Pages > Source: branch `main`, folder `/ (root)`.
3. Alamat situs akan tampil di halaman itu. Langkah dan tampilan menu GitHub bisa berubah; cek dokumentasi GitHub Pages.
Alternatif: Netlify atau Cloudflare Pages (unggah folder ini).

## Sebelum dipublikasikan
- Periksa syarat penggunaan FotMob (belum diverifikasi).
- Tambahkan institusi/mata kuliah di footer (`index.html`) bila perlu.
