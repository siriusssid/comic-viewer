# Comic Vertical Reader

Tools sederhana untuk membaca komik / manga dari file ZIP secara **vertikal** (seperti webtoon), dengan dukungan **split screen teks**.

Cocok dijalankan di **GitHub Pages** (100% static, client-side only).

## Fitur

- Tampilkan gambar berurutan dari atas ke bawah
- Natural sort nama file (`1, 2, 10…`)
- Support hampir semua format gambar: **JPG, PNG, WEBP, GIF, AVIF, BMP, TIFF, HEIC, SVG**, dll.
- Support file lokal `.zip` / `.cbz` (drag & drop)
- Coba support link Google Drive & URL ZIP langsung
- **Split screen**: panel teks di samping (atau bawah di mobile)
  - Tempel link **Google Docs** (export otomatis ke teks)
  - Atau upload file **.txt**
- Progress indicator + nomor halaman
- Panel teks bisa di-resize (drag handle)
- Dark mode, responsif mobile
- Tidak ada server — semua proses di browser

## Cara Deploy ke GitHub Pages

1. Buat repository baru di GitHub
2. Upload `index.html`
3. Settings → Pages → Source: Deploy from a branch → `main` / `root`
4. Buka `https://username.github.io/nama-repo`

Atau cukup buka `index.html` langsung di browser.

## Cara Pakai

### Membuka komik
1. **Paling reliable**: Download ZIP dari Google Drive → klik tombol **ZIP** / drag & drop
2. Atau tempel link Google Drive (file harus “Anyone with the link”)

### Panel teks (split screen)
1. Klik tombol **📝 Teks** di header
2. Tempel link Google Docs yang sudah di-set public, lalu klik **Muat**
3. Atau klik **Upload TXT** untuk file teks lokal

Google Docs harus di-share sebagai **Anyone with the link** (Viewer). Tools akan mencoba mengambil versi plain text-nya.

## Format yang didukung

| Jenis | Format |
|-------|--------|
| Arsip | `.zip`, `.cbz` |
| Gambar | JPG, PNG, WEBP, GIF, **AVIF**, BMP, TIFF, HEIC/HEIF, SVG, APNG, dll. |
| Teks | Google Docs (export TXT), file `.txt` |

> Catatan: Dukungan decoding gambar bergantung pada browser. AVIF didukung di Chrome, Firefox, Edge, Safari modern.

## Teknologi

- Vanilla HTML / CSS / JS
- [JSZip](https://stuk.github.io/jszip/) (CDN)

## License

MIT
