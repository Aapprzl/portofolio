# Portofolio — Muh. Aprizal

Situs portofolio pribadi satu halaman (HTML + Tailwind CSS 4), diterbitkan melalui GitHub Pages di
**https://aapprzl.github.io/portofolio/**

## Isi situs

| Bagian | Isi |
|---|---|
| Hero | Nama, peran (Teknisi Jaringan & IT Support · Web Developer · AI Agent Engineer), ringkasan profil |
| Tentang Saya | Pengalaman jaringan (±300 pelanggan, Kec. Bontocani), proyek mandiri, skripsi R&D |
| Portofolio | 3 proyek: Tarbiyyat al-Lughah, PBA 2022, Canxine Zero + daftar proyek berjalan |
| Keahlian | Jaringan, web & backend, AI & otomasi, sistem & multimedia; bahasa; penghargaan & pelatihan |
| Kontak | Email (satu-satunya kanal yang dipublikasikan) |

Semua fakta di situs berasal dari sumber data proyek pencarian kerja (`~/Documents/EARLY_JOB`),
terutama `01_profil-master/profil-master.md`. Tidak ada klaim yang tidak ada di sana.

## Struktur berkas

```
index.html          ← satu halaman, semua bagian
src/input.css       ← sumber Tailwind + aturan dasar (scroll-padding, navbar-fixed, hamburger)
src/output.css      ← hasil build, dipakai langsung oleh index.html
dist/js/script.js   ← navbar fixed saat scroll + tombol hamburger
img/                ← foto profil, tangkapan layar proyek
```

## Build CSS

```bash
npm install
npx @tailwindcss/cli -i src/input.css -o src/output.css
```

Tailwind 4 memindai `index.html` secara otomatis. Setiap kali kelas di `index.html` diubah,
`src/output.css` harus di-build ulang, lalu hasil build ikut di-commit.

## Kritik isi

- Jangan menambah bagian klien/log atau riset yang tidak dapat dibuktikan.
- Jangan menyalin nomor identitas (NIK, KK, NIM, nomor rekening) ke halaman.
- Data pribadi yang tampil di situs saat ini: email profesional dan alamat domisili.
