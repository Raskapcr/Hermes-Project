# Raska — Ekonomi Indonesia 2026

Website statis yang menjelaskan perkembangan ekonomi Indonesia tahun 2026.

## Isi

- **Ringkasan Makro** — pertumbuhan ekonomi (Q3-2026: +5,47%)
- **Inflasi & Mata Uang** — inflasi, target BI, tingkat suku bunga, nilai tukar Rupiah
- **Neraca Perdagangan** — surplus, ekspor/ impor, kontribusi komoditas
- **Peta Waktu** — kronologi Q1–Q4 2026
- **Grafik interaktif** — PDB vs inflasi (Chart.js)

## Cara menjalankan

Cara 1 — langsung dari browser:
Buka `index.html` dengan browser (double-click atau `xdg-open index.html`).

Cara 2 — pakai HTTP lokal (saran untuk browsing modern):
```bash
cd rasy-ekonomi
python3 -m http.server 8000
# kunjungi http://localhost:8000
```

Cara 3 — pakai Docker:
```bash
docker build -t rasy-ekonomi:latest .
docker run -p 8080:80 rasy-ekonomi:latest
# kunjungi http://localhost:8080
```

## Sumber data (singkat)

- Bank Indonesia (BI) — Monetary Policy Report QIII 2026
- Badan Pusat Statistik (BPS) — data pertumbuhan makro
- OECD Economic Outlook Vol.2026/1
- World Bank Indonesia Economic Prospects Jun 2026
- ADB, Kemenkeu, CNBC Indonesia, Kemendag

## Struktur file

```
index.html      # halaman utama (CSS/JS tersemat)
README.md       # dokumentasi
```

## Privileged data yang disertakan

- Pertumbuhan PDB Q1: 5,61% | Q3: 5,47%
- Inflasi April: 2,42% | Juni: 3,3%
- Suku bunga BI: 5,75%
- Kurs USD/Rp: Rp18.239 (12 Nov 2026)
- Surplus perdagangan September: US$3,36 miliar
