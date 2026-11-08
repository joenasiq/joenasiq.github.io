# Portofolio — Arjuna Satria Hutama

Web portofolio one-page untuk apply magang. Dibuat dengan HTML/CSS/JS murni (tanpa framework, tanpa template).

## Struktur

```
index.html          → halaman utama (semua konten di sini)
css/style.css       → seluruh styling
js/main.js          → interaksi (nav, mobile menu, scroll reveal)
img/                → foto profil, screenshot project
CV_Arjuna_Satria_Hutama.pdf  → dipakai tombol "Download CV" (jangan dihapus)
```

## Menjalankan lokal

Cukup buka `index.html` di browser (double-click), atau jalankan:

```
python -m http.server 8734
```

lalu buka http://localhost:8734

## Deploy ke GitHub Pages

1. Buat repo baru di GitHub (nama bebas, mis. `portfolio`), **public**.
2. Push folder ini ke repo:
   ```
   git init
   git add .
   git commit -m "Portfolio site"
   git branch -M main
   git remote add origin https://github.com/joenasiq/portfolio.git
   git push -u origin main
   ```
3. Di GitHub: **Settings → Pages → Build and deployment** → Source: **Deploy from a branch** → Branch: `main`, folder `/ (root)` → Save.
4. Dalam ~1 menit site live di `https://joenasiq.github.io/portfolio/`.

> Catatan: file `CV_Arjuna_Satria_Hutama.pdf` sengaja ikut di-push karena tombol
> "Download CV" menunjuk ke file itu. File lain di folder ini (CV .docx/.md, banner
> LinkedIn) tidak dipakai site — boleh dihapus dari repo jika tidak ingin publik.

## Mengubah konten

Semua teks ada di `index.html` (cari section-nya: Hero, About, Skills, Projects,
Experience, Contact). Warna dan font ada di bagian `:root` dalam `css/style.css`.
