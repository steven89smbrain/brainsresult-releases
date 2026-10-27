# 6. Dipakai bersama di kantor

Beberapa komputer bisa memakai **server database MySQL** yang sama: semua orang melihat tugas dan keuangan yang sama, masing-masing dengan akunnya.

## Yang dibutuhkan

- Server MySQL 8 (di kantor, VPS, atau layanan terkelola) dengan satu database kosong dan pengguna MySQL yang boleh membuat database.
- Untuk server di internet: koneksi terenkripsi (SSL / TLS). BrainsResult menawarkan *Verify* (memeriksa sertifikat) secara bawaan.
- Penyimpanan file bersama untuk Attachments & Notes: folder jaringan, S3 (mis. DigitalOcean Spaces) atau WebDAV (mis. Nextcloud).
- **Lisensi.** Tanpa lisensi, workspace di server hanya bisa dilihat. Selama beta, minta lisensi beta (lihat bawah).

## Menyiapkan

1. Komputer pertama: wizard → *Database server* (atau *Manage workspaces* → *Connections* → *Connect to a database server…*), isi host, port, database, pengguna, password, keamanan. Buat akun administrator.
2. *Manage workspaces* → *License* → masukkan lisensi beta.
3. *Manage workspaces* → *Users*: tambahkan orang, pilih akses per workspace (*Member* atau *Viewer* = hanya melihat). *Sign-in security*: berapa lama login berlaku, *Keep me signed in*, keluar otomatis saat tidak dipakai.
4. Komputer lain: *Connect to a database server…* dengan alamat yang sama, lalu login dengan akun masing-masing.

## Fitur tim (lisensi Team)

- **Siapa yang melihat:** batasi tugas, proyek, akun keuangan atau folder ke orang tertentu.
- **Peran & fitur per anggota:** Viewer, atau buka hanya Tasks / Finance untuk seseorang (*Manage features* → *Member access*).
- **Satu orang mengedit dalam satu waktu:** item yang sedang diedit orang lain terkunci sementara.
- **Komentar** (dengan `@username`) dan **penanggung jawab** tugas.

## Lisensi beta

[Buat issue](https://github.com/steven89smbrain/brainsresult-releases/issues/new/choose) berjudul *Lisensi beta*, sebutkan jumlah pengguna dan **installation id** (*Manage workspaces* → *License* → *Copy installation id*, saat server itu terbuka). Anda menerima teks lisensi `BRL1.…`; tempel di *Enter a license*.

## Catatan

- Perbarui semua komputer ke versi BrainsResult yang sama.
- Backup server database Anda sendiri juga, selain backup dari aplikasi.
