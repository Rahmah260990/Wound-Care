# Luka Pintar KKM

Prototaip antaramuka React untuk penilaian luka menggunakan rangka kerja T.I.M.E.

> **Penting:** Analisis AI dalam versi ini ialah simulasi menggunakan `setTimeout` dan data contoh. Ia belum disambungkan kepada model AI, pangkalan data, sistem autentikasi atau rekod klinikal sebenar. Jangan gunakan data pesakit sebenar pada GitHub Pages awam.

## Jalankan di komputer

Keperluan: Node.js 22 atau versi LTS semasa.

```bash
npm install
npm run dev
```

Buka alamat yang dipaparkan oleh Vite, biasanya `http://localhost:5173`.

## Bina versi production

```bash
npm run build
npm run preview
```

## Muat naik ke GitHub

1. Cipta repository baharu di GitHub.
2. Muat naik semua fail projek ini ke branch `main`.
3. Di repository, buka **Settings → Pages**.
4. Pada **Build and deployment → Source**, pilih **GitHub Actions**.
5. Push ke `main`. Workflow `.github/workflows/deploy.yml` akan membina dan menerbitkan laman.

Konfigurasi Vite akan mengesan nama repository secara automatik semasa GitHub Actions berjalan, jadi aset berfungsi pada URL berbentuk `https://USERNAME.github.io/NAMA-REPOSITORY/`.

## Struktur utama

- `src/App.jsx` — aplikasi asal yang telah disesuaikan kepada projek React.
- `src/index.css` — Tailwind CSS, font dan animasi.
- `vite.config.js` — konfigurasi Vite dan GitHub Pages.
- `.github/workflows/deploy.yml` — deployment automatik ke GitHub Pages.

## Sebelum penggunaan klinikal sebenar

Perlu ditambah sekurang-kurangnya:

- autentikasi dan kawalan akses;
- backend/API serta pangkalan data selamat;
- penyulitan data ketika penghantaran dan penyimpanan;
- audit trail, consent dan polisi retention;
- validasi klinikal model AI;
- semakan keselamatan siber dan pematuhan dasar organisasi;
- mekanisme semakan serta pengesahan oleh pegawai klinikal.
