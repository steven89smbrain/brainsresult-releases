# 1. Instalasi & mulai

## Memasang

1. Unduh `brainsresult-<versi>-setup.exe` dari halaman [Releases](https://github.com/steven89smbrain/brainsresult-releases/releases/latest).
2. Jalankan. Bila muncul **"Windows protected your PC"** (SmartScreen), klik *More info* → *Run anyway*. Peringatan ini muncul karena installer beta belum ditandatangani.
3. Baca dan setujui perjanjian lisensi, pilih folder instalasi, selesai. Shortcut dibuat di Desktop dan Start menu.

Sistem: Windows 10 / 11 64-bit, ± 500 MB ruang disk.

## Wizard pertama

Saat pertama dibuka, wizard menanyakan:

| Langkah | Pilihan |
|---|---|
| **Database** | *This computer* (SQLite, untuk pribadi) atau *Database server* (MySQL, untuk kantor — lihat [bagian 6](06-kantor.md)). Untuk server ada *Test connection* |
| **Data folder** | Folder tempat data, backup dan file disimpan. Pilih folder yang ikut Anda cadangkan (mis. di drive D:) |
| **Sign-in** | Opsional: wajibkan login dengan akun administrator. Disarankan bila komputer dipakai bersama |
| **Workspace** | Nama workspace pertama, dan opsi **workspace contoh** berisi data latihan |
| **Review** | Periksa, lalu *Finish setup* |

## Di mana data saya?

Data ada di **folder data** yang Anda pilih (atau di server database Anda), **bukan** di folder program. Update dan instal ulang tidak menghapusnya. Pengaturan komputer ada di `%APPDATA%\BrainsResult`.

## Update

BrainsResult memeriksa versi baru sendiri (Settings → *Updates* → *Check for updates* untuk memeriksa sekarang), mengunduhnya di belakang layar, lalu memasangnya saat Anda menekan *Restart now* atau menutup aplikasi.

## Berjalan di tray

Menutup jendela tidak mematikan BrainsResult: ia tetap di tray (dekat jam) agar pengingat tetap muncul. Keluar lewat menu ikon tray → *Quit BrainsResult*. Perilaku ini dan *Start with Windows* diatur di Settings.

## Mencopot

Settings Windows → Apps → BrainsResult → *Uninstall*. Data Anda **tetap ada**; hapus folder data sendiri bila memang ingin.
