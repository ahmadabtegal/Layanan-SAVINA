# SAVINA — Saluran Virtual Perizinan DPMPTSP Kota Tegal

Paket frontend statis berdasarkan file HTML SAVINA terakhir yang diberikan. Logo dipisahkan ke folder `assets/` agar mudah dikelola dan tidak tertanam sebagai gambar base64 di HTML.

## Struktur folder

```text
savina-github-pages/
├── index.html
├── README.md
└── assets/
    ├── logo-savina.png
    ├── logo-dpmptsp.png
    ├── logo-kota-tegal.png
    └── favicon.png
```

## Penyesuaian logo

- Logo utama SAVINA memakai `assets/logo-savina.png`.
- Logo DPMPTSP dan lambang Kota Tegal memakai file terpisah di `assets/`.
- Tinggi logo di area header diseragamkan agar sejajar; ukuran gambar tetap proporsional dan tidak diregangkan. Pada layar kecil, tinggi logo diperkecil secara responsif.
- Untuk mengganti logo, pertahankan nama file atau ubah jalur aset pada `index.html`.

## Deploy ke GitHub Pages

1. Ekstrak ZIP ini.
2. Unggah `index.html`, `README.md`, dan folder `assets/` ke root repository GitHub.
3. Buka **Settings → Pages**.
4. Pilih **Deploy from a branch**, branch `main`, folder `/(root)`, lalu **Save**.

## Catatan backend

GitHub Pages hanya menyajikan frontend. Fitur SAVINA yang memerlukan data, autentikasi, penyimpanan, atau layanan eksternal tetap membutuhkan endpoint/backend yang sudah dikonfigurasi di HTML. Periksa URL endpoint dan izin akses sebelum digunakan.
