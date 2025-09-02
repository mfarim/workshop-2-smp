# Pengenalan CSS (Cascading Style Sheets)

CSS adalah bahasa yang digunakan untuk mengatur tampilan dan layout halaman web. CSS bekerja dengan cara memberikan style pada elemen HTML.

## 1. Apa itu CSS?
CSS (Cascading Style Sheets) adalah bahasa stylesheet yang digunakan untuk:
- Mengatur warna, font, dan ukuran teks
- Mengatur layout dan posisi elemen
- Menambahkan animasi dan efek visual
- Membuat desain yang responsif

---

## 2. Cara Menggunakan CSS

### a. Inline CSS
CSS yang ditulis langsung di dalam atribut `style` pada elemen HTML.
```html
<p style="color: blue; font-size: 18px;">Teks ini berwarna biru</p>
```

### b. Internal CSS
CSS yang ditulis di dalam tag `<style>` di bagian `<head>`.
```html
<head>
  <style>
    p {
      color: blue;
      font-size: 18px;
    }
  </style>
</head>
```

### c. External CSS
CSS yang ditulis di file terpisah (file .css) dan dihubungkan ke HTML.
```html
<head>
  <link rel="stylesheet" href="style.css">
</head>
```

---

## 3. Tailwind CSS

Tailwind CSS adalah framework CSS yang menggunakan pendekatan utility-first. Alih-alih menulis CSS custom, kita menggunakan class-class yang sudah disediakan.

### Keunggulan Tailwind CSS:
- **Utility-first**: Class-class kecil dan spesifik
- **Responsive**: Mudah membuat desain responsif
- **Customizable**: Dapat dikustomisasi sesuai kebutuhan
- **Fast Development**: Mempercepat proses development

### Cara Menambahkan Tailwind CSS:
```html
<script src="https://cdn.tailwindcss.com"></script>
```

---

## 4. Contoh Penggunaan Tailwind CSS

### a. Styling Text
```html
<!-- Ukuran dan warna teks -->
<h1 class="text-3xl font-bold text-blue-600">Judul Besar</h1>
<p class="text-lg text-gray-700">Paragraf dengan teks abu-abu</p>

<!-- Text alignment -->
<p class="text-center">Teks di tengah</p>
<p class="text-right">Teks di kanan</p>
```

### b. Layout dan Spacing
```html
<!-- Margin dan Padding -->
<div class="m-4 p-6">Margin 4 dan Padding 6</div>
<div class="mx-auto max-w-4xl">Centered dengan lebar maksimal</div>

<!-- Flexbox -->
<div class="flex justify-center items-center space-x-4">
  <button class="bg-blue-500 text-white px-4 py-2">Button 1</button>
  <button class="bg-green-500 text-white px-4 py-2">Button 2</button>
</div>
```

### c. Background dan Border
```html
<!-- Background -->
<div class="bg-gray-100">Background abu-abu terang</div>
<div class="bg-blue-600 text-white">Background biru dengan teks putih</div>

<!-- Border dan Rounded -->
<div class="border border-gray-300 rounded-lg p-4">
  Kotak dengan border dan sudut melengkung
</div>
```

### d. Responsive Design
```html
<!-- Responsive text size -->
<h1 class="text-lg md:text-2xl lg:text-4xl">
  Ukuran teks yang responsif
</h1>

<!-- Responsive layout -->
<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
  <div>Item 1</div>
  <div>Item 2</div>
  <div>Item 3</div>
</div>
```

### e. Hover Effects
```html
<!-- Hover pada button -->
<button class="bg-blue-500 hover:bg-blue-700 text-white px-4 py-2 rounded">
  Hover Button
</button>

<!-- Hover pada link -->
<a href="#" class="text-blue-600 hover:text-blue-800 hover:underline">
  Link dengan hover effect
</a>
```

---

## 5. Contoh Implementasi di Project

Berikut contoh penggunaan Tailwind CSS pada biodata diri:

```html
<!-- Navigation -->
<nav class="bg-blue-600 text-white p-4 shadow-md">
  <div class="container mx-auto flex justify-center space-x-6">
    <a href="#" class="hover:text-blue-200 transition">Beranda</a>
    <a href="#" class="hover:text-blue-200 transition">Tentang</a>
  </div>
</nav>

<!-- Main Content -->
<main class="max-w-4xl mx-auto p-6 bg-white shadow-lg rounded-lg my-8">
  <header class="text-center mb-8">
    <h1 class="text-3xl font-bold text-gray-800">Biodata Diri</h1>
  </header>
  
  <!-- Table -->
  <table class="w-full border-collapse border border-gray-300">
    <tr class="bg-gray-50">
      <td class="border border-gray-300 p-3 font-medium">Nama</td>
      <td class="border border-gray-300 p-3">: John Doe</td>
    </tr>
  </table>
</main>
```

---

## 6. Tips Menggunakan Tailwind CSS

1. **Gunakan container**: `container mx-auto` untuk membuat layout yang centered
2. **Responsive prefix**: `sm:`, `md:`, `lg:`, `xl:` untuk breakpoint
3. **Spacing system**: Gunakan scale 4 (1rem) sebagai dasar spacing
4. **Color system**: Gunakan skala 50-900 untuk variasi warna
5. **Combine classes**: Gabungkan multiple utility untuk hasil yang diinginkan

### Contoh Responsive Card:
```html
<div class="bg-white rounded-lg shadow-md p-6 m-4 transition hover:shadow-lg">
  <img class="w-full h-48 object-cover rounded-md mb-4" src="image.jpg">
  <h3 class="text-xl font-semibold mb-2">Card Title</h3>
  <p class="text-gray-600 mb-4">Card description text here.</p>
  <button class="bg-blue-500 hover:bg-blue-700 text-white px-4 py-2 rounded">
    Read More
  </button>
</div>
```

---