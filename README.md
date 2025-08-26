# Penjelasan Tag HTML

## 1. `<!DOCTYPE html>`
Mendefinisikan tipe dokumen HTML5. Ini memberitahu browser bahwa file ini adalah dokumen HTML versi terbaru.

---

## 2. `<html lang="id">`
Tag utama pembuka dan penutup dokumen HTML.
- `lang="id"`: Menandakan bahwa bahasa utama halaman ini adalah Bahasa Indonesia.

---

## 3. `<head> ... </head>`
Bagian ini berisi metadata tentang dokumen, bukan konten yang ditampilkan ke pengguna.
- `<meta charset="UTF-8" />`: Mengatur encoding karakter menjadi UTF-8.
- `<meta name="viewport" ...>`: Membuat tampilan responsif di perangkat mobile.
- `<title>...</title>`: Judul halaman, muncul di tab browser.
- `<meta name="description" ...>`: Deskripsi halaman untuk mesin pencari (SEO).

---

## 4. `<body> ... </body>`
Semua konten yang ditampilkan pada halaman web berada di dalam tag ini.

---

### a. `<nav> ... </nav>`
Bagian navigasi utama situs.  
Berisi tautan seperti:
- Beranda (`<a href="/">`)
- Tentang (`<a href="/about">`)
- Kontak (`<a href="/contact">`)

---

### b. `<main> ... </main>`
Bagian utama konten halaman.  

#### - `<header> ... </header>`
Berisi judul utama dan sambutan.

#### - `<section> ... </section>`
Bagian untuk memisahkan konten berdasarkan topik.
- Paragraf tentang profil dan pengalaman pemilik situs.
- Daftar link ke situs eksternal (Google, Facebook, Twitter).

#### - `<aside> ... </aside>`
Biasanya untuk informasi tambahan atau promosi (misal: portofolio).

---

### c. `<footer> ... </footer>`
Bagian bawah halaman, biasanya untuk hak cipta, tautan, dan keterangan tambahan.

---