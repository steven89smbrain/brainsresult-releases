# 5. Backup & pindah komputer

## Backup manual

*Manage workspaces* → *Backup & restore* → *Back up…*: pilih workspace dan tempat menyimpan. Hasilnya satu file `.brbackup` berisi data dan file workspace. Bisa diberi **password** (dienkripsi AES-256); password yang hilang tidak bisa dipulihkan.

## Backup otomatis

Di tempat yang sama: jadwal (harian / mingguan), folder tujuan (sebaiknya drive lain atau folder yang disinkronkan ke cloud), jumlah backup yang disimpan, dan password opsional. Bila backup gagal, Anda diberi tahu di inbox.

## Restore

*Restore…* → pilih file `.brbackup` → pulihkan sebagai **workspace baru**, atau **ganti** workspace yang ada (yang lama tidak dihapus: diganti nama "… (before restore …)" dan diarsipkan).

## Pindah ke komputer baru

1. Di komputer lama: backup semua workspace.
2. Pasang BrainsResult di komputer baru, selesaikan wizard.
3. *Restore…* setiap file backup.

Bila memakai server database kantor, cukup pasang aplikasi dan sambungkan ke server yang sama (lihat [bagian 6](06-kantor.md)).

## Saran

- Simpan backup di luar komputer (drive eksternal / cloud).
- Coba restore sesekali, agar yakin backup bisa dipakai.
- Sebelum memperbarui struktur data, BrainsResult otomatis menyimpan salinan database lokal di folder `backups`.
