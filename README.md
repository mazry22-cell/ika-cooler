# IKA Sewa Air Cooler — website

Laman satu halaman untuk bio link. Statik sepenuhnya: tiada PHP, tiada database, tiada CDN.

## Fail

| Fail | Guna |
|---|---|
| `index.html` | Halaman utama (harga, spesifikasi, kawasan, FAQ) |
| `links.html` | Halaman pautan gaya link-in-bio (3 butang) |
| `404.html` | Halaman ralat GitHub Pages |
| `img/cooler.webp` | Gambar produk |
| `img/logo-white.png` | Logo untuk latar gelap |
| `img/logo-navy.png` | Logo untuk latar cerah |
| `img/icon.png`, `img/favicon-32.png`, `img/apple-touch-icon.png` | Ikon |
| `img/og.jpg` | Gambar preview 1200×630 bila link dikongsi |

## Nombor WhatsApp

`60111201708` — ada di **6 tempat** dalam `index.html` (1 JSON-LD `telephone` + 5 pautan `wa.me`) dan **1 tempat** dalam `links.html`.
Teks paparan `011-1120 1708` ada **1 tempat** dalam footer `index.html`.
Kalau nombor bertukar: Ctrl+H / Cari & Ganti, ganti kedua-dua format.

URL penuh `https://mazry22-cell.github.io/ika-cooler/` ada dalam `<head>` (canonical, `og:image`, `og:url`) dan JSON-LD. Kalau tukar nama repo atau domain, ganti di situ, kalau tidak preview WhatsApp/Facebook tak keluar.

## Cara letak di GitHub Pages (tanpa terminal)

1. Buat repo baru di GitHub: nama `ika-cooler`, **Public**, jangan tambah README.
2. Dalam repo, tekan **Add file → Upload files**. Seret **semua isi folder ini** (termasuk folder `img`), bukan folder luarnya.
3. Tekan **Commit changes**.
4. Pergi **Settings → Pages**. Di bawah *Build and deployment*, pilih **Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
5. Tunggu 1–2 minit. URL akan jadi `https://mazry22-cell.github.io/ika-cooler/`
6. Halaman pautan: `https://mazry22-cell.github.io/ika-cooler/links.html`

Kalau awak guna nama repo lain, URL ikut nama itu.

## Nota

- `.nojekyll` membolehkan fail bermula dengan `_` dihidangkan. Jangan buang.
- `links.html` ada `noindex` supaya Google fokus pada `index.html`.
- Tiada analitik dipasang. Kalau nak tahu berapa orang tekan WhatsApp, tambah pembilang sendiri kemudian.
