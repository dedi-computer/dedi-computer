# Dedi Computer - Website Portofolio

Website portofolio resmi **Dedi Computer** — Jasa servis elektronik di Alam Barajo, Jambi.

**Isi:**
- `index.html` — Halaman utama (responsive, SEO meta tags, form pemesanan).
- `favicon.ico` — Ikon situs.
- `README.md` — Deskripsi dan petunjuk deploy ke GitHub Pages.

## Cara deploy ke GitHub Pages
1. Buat repository baru (misal: `dedi-computer`) di GitHub.
2. Upload seluruh isi folder ini ke branch `main`.
3. Di GitHub, buka **Settings → Pages**, pilih **Deploy from a branch**, pilih `main` dan folder `/ (root)`.
4. Setelah beberapa menit, website akan tersedia di: `https://<username>.github.io/dedi-computer`

## Catatan teknis
- Tombol *Kirim via WhatsApp* membuka chat ke +62 823-7173-1189 dengan format pesan otomatis.
- Tombol *Kirim via Email* menggunakan Formspree. Jika ingin gunakan email lain, buat endpoint Formspree dan ganti `FORMSPREE_ENDPOINT` di `index.html`.
- Untuk mengganti nomor telepon, ubah juga nomor di `index.html` (semua instance 082371731189 / wa link 6282371731189).

Jika mau, saya bisa bantu langsung upload (kalau kamu berikan akses) atau beri panduan langkah demi langkah saat kamu siap.
