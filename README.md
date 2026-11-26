# Jurnal Ilmiah Proyek 2 - Coneckin

Naskah jurnal ilmiah untuk Proyek 2 Program Studi Sarjana Terapan Teknik Informatika, Universitas Logistik dan Bisnis Internasional (ULBI) menggunakan LaTeX dengan standar format IEEE.

Disusun sesuai dengan kriteria [Project Instruction](https://ll.my.id/instruction/).

## Judul Artikel
**Rancang Bangun Coneckin: Otomasi Autentikasi Captive Portal Kampus Berbasis Android dengan Arsitektur Kredensial Terenkripsi**

## Struktur Berkas

```
jurnal/
├── .github/
│   └── workflows/
│       └── release.yml        # CI/CD otomatis: compile LaTeX & auto release PDF
├── figures/                   # Gambar & diagram arsitektur
├── references.bib             # Daftar pustaka (BibTeX IEEE format)
├── main.tex                   # Dokumen induk LaTeX artikel 2 kolom
├── compile-latex.ps1          # Script kompilasi lokal Windows PowerShell
└── README.md
```

## Alur Kerja Otomatisasi (CI/CD)

Setiap perubahan pada cabang `main` akan:
1. Menjalankan GitHub Actions workflow `release.yml`.
2. Mengompilasi naskah `main.tex` ke format PDF menggunakan TeXLive.
3. Menghasilkan tag rilis otomatis `v1.0.<nomor_build>`.
4. Menerbitkan rilis baru di GitHub Releases dengan menyertakan `Jurnal-Proyek2-Coneckin.pdf`.
