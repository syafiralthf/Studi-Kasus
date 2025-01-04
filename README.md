## Biodata
Nama : Syafira Luyhfi Azzahra

Kelas : TI.24.A.4

NIM : 312410353

# Validasi Input Pendaftaran Online
Program ini dibuat untuk memvalidasi data input pada proses pendaftaran online. Validasi dilakukan pada tiga jenis data: nama lengkap, nomor telepon, dan email. Program ini memberikan pesan kesalahan yang spesifik jika ada input yang tidak valid dan menyatakan bahwa data pendaftaran valid jika semua input benar.

## Cara Kerja Program
1. Validasi Nama

![validasinama](https://github.com/user-attachments/assets/22161cf2-4c42-4d42-99c1-0175a46a2391)

Penjelasan:

- Fungsi isalpha() memastikan bahwa name hanya terdiri dari huruf.
- Jika nama berisi angka, spasi, atau karakter khusus, validasi akan gagal, dan pesan error ditambahkan ke daftar errors.

2. Validasi Nomor Telepon

![validasitelepon](https://github.com/user-attachments/assets/d14f95b3-b353-4907-b4ab-54dc9b936f9d)

Penjelasan:

- Fungsi isdigit() memastikan bahwa phone hanya terdiri dari angka.
- Jika phone berisi huruf, spasi, atau karakter lain, validasi akan gagal.

3. Validasi Email

![validasiemail](https://github.com/user-attachments/assets/7c677ba5-dc0c-489a-8100-c627381bcd25)

Penjelasan:

- Ekspresi reguler ^\S+@\S+\.\S+$ memastikan bahwa:
  - Ada karakter sebelum @ (\S+ berarti non-spasi).
  - Ada karakter sebelum dan sesudah ..
  - Tidak ada spasi di seluruh string email.
- Jika format email tidak sesuai, validasi akan gagal.

4. Hasil Validasi

![outputhasilvalidasi](https://github.com/user-attachments/assets/cf3beeaa-35cc-4599-953a-668e4b2be91b)

Penjelasan:

- Jika ada elemen dalam daftar errors, setiap pesan kesalahan akan ditampilkan.
- Jika tidak ada kesalahan, program akan menampilkan "Data pendaftaran valid."

## Persyaratan
- Python 3.x
- Libary re (sudah termasuk dalam python standar)

## Cara Menjalankan Program
1. Clone repositori ini atau salin file program ke komputer Anda.
2. Buka terminal atau command prompt.
3. Jalankan program menggunakan perintah: bash python nama_file.py
4. Masukkan data sesuai dengan permintaan program:
   - Nama lengkap
   - Nomor telepon
   - Email
5. Program akan menampilkan hasil validasi:
   - Pesan "Data pendaftaran valid" jika semua input benar.
   - Pesan kesalahan untuk setiap data yang tidak valid.

## Input & Output

## Input

![code (1)](https://github.com/user-attachments/assets/98f89e97-aa84-4960-9929-2593f4ee26f5)

## Output Valid

![{CE41B4E6-ABA6-46C4-B26C-20767879B279}](https://github.com/user-attachments/assets/33a69ef9-45f0-4457-b9cc-dee6cab6b40d)

## Input Tidak Valid

![{BC4452B2-ED17-4326-B93B-A51FF992606F}](https://github.com/user-attachments/assets/2877b04b-4b85-4856-8103-250f6f67a175)

## Fitur dan Kemampuan
- Kesesuaian dengan berbagai pengguna
- Dapat Dimodifikasi
- Keamanan dasar input
- Laporan kesalahan yang spesifik
