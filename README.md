# Portfolio

Proyek ini merupakan portofolio pribadi yang dibuat menggunakan [Astro](https://astro.build/), [Vue](https://vuejs.org/), dan [Tailwind CSS](https://tailwindcss.com/). Repositori ini menyajikan contoh sederhana bagaimana membangun situs statis modern dengan komponen interaktif.

## Stack
- **Astro** sebagai static site builder
- **Vue 3** untuk komponen interaktif
- **Tailwind CSS** untuk styling

## Prasyarat
- [Node.js](https://nodejs.org/) versi 18 atau lebih baru
- npm (disertakan bersama Node.js)

## Instalasi
1. Klona repository:
   ```bash
   git clone <url-repo-anda>
   cd portfolio
   ```
2. Pasang dependensi:
   ```bash
   npm install
   ```

## Development
Jalankan server pengembangan untuk melihat perubahan secara langsung:
```bash
npm run dev
```
Server akan berjalan di `http://localhost:4321` secara default.

## Build dan Deploy
1. Bangun proyek untuk produksi:
   ```bash
   npm run build
   ```
   Hasil build akan berada di folder `dist/`.
2. Untuk pratinjau build secara lokal:
   ```bash
   npm run preview
   ```
3. Deploy folder `dist/` ke penyedia hosting statis favorit Anda (mis. Vercel, Netlify, GitHub Pages, dll.).

Selamat berkarya!
