# MH Tour V8 — Android GitHub Ready

Aplikasi Android audio streaming untuk Muthawwif/Guide dan Jemaah.

## Struktur repository

Upload **isi folder ini** ke root repository GitHub, bukan folder induknya.

```text
MH-Tour/
├── .github/
│   └── workflows/
│       └── build-apk.yml
├── app/
├── build.gradle
├── settings.gradle
├── gradle.properties
├── .gitignore
└── README.md
```

## Peran aplikasi

### Guide / Muthawwif
- Akses MIC Live.
- Membuat kode grup.
- Menampilkan QR koneksi.
- Menyiarkan audio ke banyak Jemaah.
- Melihat jumlah koneksi.

### Jemaah
- Hanya pendengar.
- Tidak ada tombol MIC.
- Tidak meminta izin microphone.
- Scan QR atau masukkan kode grup.
- Streaming otomatis setelah Guide ditemukan.

## Build APK di GitHub

1. Buat repository baru bernama `MH-Tour`.
2. Upload **semua isi folder project ini** sehingga `.github` berada di root repository.
3. Commit ke branch `main` atau `master`.
4. Buka tab **Actions**.
5. Pilih **Build MH Tour APK**.
6. Klik **Run workflow** jika workflow belum berjalan otomatis.
7. Setelah selesai, buka hasil workflow dan download artifact **MH-Tour-V8-release**.

Workflow menggunakan Gradle 8.10.2 melalui GitHub Actions sehingga repository tidak membutuhkan Gradle Wrapper untuk menjalankan build.

## Catatan jaringan

Guide dan Jemaah harus berada pada Wi-Fi/hotspot yang mengizinkan komunikasi antar-perangkat. Untuk rombongan besar, gunakan access point/router yang mengizinkan client-to-client communication.
