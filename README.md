# Rekrut Lokal

Aplikasi rekrutmen (ATS) untuk tim kecil yang berjalan di komputer Anda sendiri.
Kelola lowongan, kandidat, penyaringan CV, wawancara, penawaran, dan laporan dalam
satu aplikasi web lokal. Tidak perlu server cloud, langganan per pengguna, atau
koneksi internet untuk fitur utamanya.

Repositori ini hanya berisi berkas rilis: installer Windows dan paket Client.
Kode sumber dan master key tidak disimpan di sini.

## Kenapa Rekrut Lokal

- **Data tetap di komputer Anda.** Database, CV, dan riwayat rekrutmen tersimpan di
  folder aplikasi, bukan di server pihak lain.
- **Tanpa biaya per pengguna.** Satu instalasi dipakai bersama tim lewat akun
  Admin, Recruiter, dan Viewer.
- **Tetap jalan tanpa internet.** Fitur inti bekerja offline; internet hanya
  dibutuhkan saat setup pertama dan bila memakai AI.
- **AI opsional dan terkendali.** Setiap pengguna memakai kunci Gemini pribadi.
  Admin menentukan apakah cloud AI boleh dipakai, dan tanpa AI aplikasi tetap
  berjalan penuh.
- **Backup terenkripsi.** Backup otomatis dan manual berformat `.age`, dengan kata
  sandi yang hanya Anda pegang.
- **Bisa dipakai di jaringan kantor.** Mode LAN membuka aplikasi untuk komputer
  lain di jaringan privat yang tepercaya.
- **Lisensi offline.** Kunci lisensi ditandatangani dan diverifikasi tanpa
  menghubungi server lisensi.

## Fitur

### Dasbor

Ringkasan pipeline, tindak lanjut yang jatuh tempo, notifikasi, dan pengingat
backup dalam satu layar.

### Lowongan dan kriteria

Setiap lowongan menyimpan kriteria wajib dan nilai plus yang menjadi dasar
penyaringan. Lowongan baru melewati requisisi dan persetujuan Admin, lengkap
dengan departemen, jumlah kebutuhan, rentang gaji, dan anggaran.

### Pipeline per lowongan

Setiap lowongan punya alur tahapnya sendiri. Atur nama, urutan, dan jeda follow-up
otomatis per tahap. Perpindahan tahap mengikuti aturan yang sah dan tercatat di
riwayat lamaran.

### Unggah CV dan impor CSV

Masukkan kandidat lewat unggahan CV (PDF/gambar) atau daftar CSV ke lowongan yang
sedang dibuka. OCR dan ekstraksi teks berjalan lokal.

### Penyaringan dan bukti

Penyaringan mencocokkan teks CV dengan kriteria lowongan, menampilkan skor,
cakupan bukti, dan kutipan CV. Hasil yang belum yakin ditandai untuk diperiksa
manual, bukan dipaksa menjadi angka.

### Wawancara dan scorecard

Atur jadwal, unduh undangan `.ics`, lalu catat penilaian pewawancara pada enam
kompetensi. Panduan wawancara bisa disusun dari kriteria lowongan.

### Penawaran kerja

Susun penawaran, ajukan persetujuan Admin, kirim, lalu catat jawaban kandidat.
Menerima penawaran otomatis memindahkan lamaran ke tahap Diterima.

### Komunikasi dan tindak lanjut

Catat pesan WhatsApp/email dan tindak lanjut agar riwayatnya tidak hilang.
Pengingat muncul di lonceng notifikasi.

### Kandidat, tag, dan talent pool

Direktori lintas lowongan untuk menemukan kembali kandidat, mencatat consent,
tag, catatan, dan keputusan talent pool.

### Laporan dan ekspor

Ukur time-to-hire, konversi antar tahap, efektivitas sumber kandidat, dan tren
bulanan. Setiap tabel bisa diekspor ke CSV. Ada juga pemeriksaan konsistensi
keputusan terhadap bukti penyaringan.

### Citra, asisten AI

Asisten opsional untuk menulis deskripsi lowongan, merangkum, dan menyiapkan bahan
wawancara. Memakai kunci Gemini pribadi pengguna; Admin mengatur izin dan filter
privasi.

### Akun, keamanan, dan pengaturan

Peran Admin, Recruiter, dan Viewer. Kata sandi dikelola sendiri, kunci AI pribadi
tidak bisa dilihat Admin, dan setiap perubahan penting masuk audit. Pengaturan
mencakup organisasi, pengguna, departemen, SMTP, retensi data, dan status sistem.

## Persyaratan

- Windows 10/11 64-bit.
- Installer sudah membawa Node.js 22, jadi tidak perlu memasang Node manual.
- Internet saat setup pertama untuk memasang komponen dan membangun aplikasi.
- Ruang disk kosong yang cukup untuk aplikasi, database, CV, dan backup.

## Pemasangan

1. Buka tab **Releases** dan pilih versi terbaru (minimal **v0.2.3**).
2. Unduh `RekrutLokal-Setup-vX.Y.Z.exe`.
3. Jalankan installer, lalu buka **RekrutLokal** dari Start Menu.
4. Pilih **Setup awal**, tunggu sampai selesai, lalu catat **Kode mesin**.
5. Aktifkan lisensi, buat Admin pertama di halaman Setup, lalu tambahkan pengguna.

## Coba gratis 7 hari

Belum punya lisensi? Setelah setup, buka halaman **Aktivasi** dan tempel kunci trial
universal ini:

```
RL1.eyJ2IjoxLCJpZCI6ImxpY180ZjYzYTU0OWFhN2FkNzk4IiwibGljZW5zZWUiOiJUcmlhbCBVbml2ZXJzYWwiLCJtYWNoaW5lIjoiKiIsInBsYW4iOiJ0cmlhbCIsImlzc3VlZEF0IjoiMjAyNi0xMS0wN1QwNTowMTo0MS40NDRaIiwiZXhwaXJlc0F0IjoiMjAyNy0xMS0wN1QwNTowMTo0MS40NDRaIiwidHJpYWxEYXlzIjo3LCJub3RlIjoiVHJpYWwgdW5pdmVyc2FsIDcgaGFyaSBzZWphayBha3RpdmFzaSJ9.Il2Vdoq8vmwr_YqKFRrPVvJSzlVhSaZkcRXtvSpeTIh9SD3oaPVLgeukuDSG45vEYSJx9kvFkMUKkGYWuBa7Bg
```

Masa trial **7 hari dihitung sejak kunci pertama kali diaktifkan** di komputer itu,
bukan sejak kunci diterbitkan. Kunci ini bisa dipakai di komputer mana pun dan masih
bisa diaktifkan sampai **7 November 2027**. Setelah trial habis, aplikasi kembali ke
halaman Aktivasi; hubungi pemilik aplikasi untuk kunci baru.

Gunakan versi **0.2.3 atau lebih baru**. Versi lama menghitung masa trial dari
tanggal kunci diterbitkan.

## Pembaruan dan rilis

Versi memakai format `vX.Y.Z`. Setiap rilis menerbitkan tiga berkas:

| Berkas | Isi |
| --- | --- |
| `RekrutLokal-Setup-vX.Y.Z.exe` | Installer Windows, sudah termasuk Node.js |
| `RekrutLokal-Client-vX.Y.Z.zip` | Paket aplikasi untuk pemasangan manual |
| `RekrutLokal-Client-vX.Y.Z-full.zip` | Paket aplikasi plus Node.js portable |

Cara memperbarui:

1. Tutup aplikasi dari launcher (**Hentikan Aplikasi**).
2. Buka **RekrutLokal.exe**, pilih **Update**.
3. Aplikasi mengunduh paket Client dari rilis terbaru di repositori ini, memasang
   dependensi, lalu membangun ulang aplikasi.
4. Setelah selesai, pilih **Jalankan Aplikasi**.

Yang selalu dipertahankan saat update: `.data` (database, CV, lisensi, pengaturan),
`.env.local`, dan folder `runtime`. Bila versi terpasang sudah sama dengan rilis
terbaru, updater berhenti tanpa mengubah berkas. Tidak perlu akun atau token GitHub.

Jika update otomatis gagal, unduh installer versi terbaru dan pasang di folder yang
sama. **Jangan menghapus `.data`**; data dan lisensi ada di sana.

## Lisensi

Aplikasi memerlukan kunci lisensi yang terikat ke kode mesin. Kirim **Kode mesin**
yang tampil di halaman Aktivasi ke pemilik aplikasi untuk mendapatkan kunci. Lisensi
memiliki tanggal kedaluwarsa; perpanjangan diterbitkan dengan kode mesin yang sama.

Kunci trial universal hanya untuk uji coba dan tidak mengunci fitur.

## Bantuan

- Port dipakai aplikasi lain: tutup aplikasi tersebut lalu jalankan lagi.
- Antivirus memblokir: izinkan folder aplikasi dan Node.js.
- SmartScreen menampilkan peringatan: installer belum ditandatangani secara digital.
  Pilih **More info**, lalu **Run anyway** hanya jika berkas diunduh dari repositori ini.
- Masalah lain: kirim log terbaru dari `.data/logs` dan salinan diagnostik dari
  halaman error kepada pemilik aplikasi.

Copyright (c) 2026 LiHenZ. Hak cipta dilindungi.
