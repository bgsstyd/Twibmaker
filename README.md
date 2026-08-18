# 🎓 TwibMaker v1.2 - Automated MPLS Twibbon Generator

[![Release](https://img.shields.io/badge/Release-v1.2.0--stable-blue.svg)](#)
[![Python 3.10+](https://img.shields.io/badge/Python-3.10+-yellow.svg)](#)
[![Platform](https://img.shields.io/badge/Platform-Windows%20x64-brightgreen.svg)](#)
[![License](https://img.shields.io/badge/License-MIT-lightgrey.svg)](#)

Aplikasi desktop otomatis untuk mempermudah peserta **Masa Pengenalan Lingkungan Sekolah (MPLS) 2026** dalam memasang bingkai *twibbon* resmi angkatan ke foto profil tanpa perlu aplikasi editing rumit seperti Photoshop atau Canva.

Aplikasi ini menggunakan modul otomatisasi grafis berbasis Python untuk menyelaraskan rasio aspek foto, meningkatkan resolusi secara instan, dan melakukan sinkronisasi *overlay frame* secara *pixel-perfect*.

---

## 📌 Cara Penggunaan (Peserta MPLS)

1. **Unduh Executable:**
   * Ambil file rilis terbaru `TwibMaker.exe` pada tab [Releases](../../releases) atau jalankan langsung versi binary yang dibagikan oleh panitia divisi IT.
2. **Siapkan Foto:**
   * Letakkan foto profil terbaik kamu di dalam folder yang sama dengan aplikasi.
   * **PENTING:** Beri nama file foto tersebut menjadi `flag.png` (Format harus `.png`).
3. **Jalankan Aplikasi:**
   * Klik ganda pada `TwibMaker.exe`.
   * Program akan otomatis melakukan kompresi resolusi, penyesuaian *chroma template*, dan mengenkapsulasi bingkai MPLS ke dalam aset foto kamu.
4. **Hasil Akhir:**
   * Tunggu hingga proses render selesai. File foto kamu akan diproses dan dioptimasi ke dalam format terproteksi `flag.png.enc` untuk siap diunggah ke portal registrasi sekolah.

---

## 🛠️ Persyaratan Sistem

* **Sistem Operasi:** Windows 10 / 11 (64-bit)
* **Format Input:** Portable Network Graphics (`.png`)
* **Dependensi:** *None (Standalone Executable via PyInstaller)*

---

## ⚙️ Building from Source

Bagi tim divisi IT / Mentor yang ingin melakukan kompilasi mandiri dari *source code* Python:

```bash
# Clone repository
git clone [https://github.com/mpls-official-2026/TwibMaker-Engine.git](https://github.com/mpls-official-2026/TwibMaker-Engine.git)
cd TwibMaker-Engine

# Install dependensi yang dibutuhkan
pip install -r requirements.txt

# Jalankan pipeline generator
python lock_asset.py
