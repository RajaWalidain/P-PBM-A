# 📱 Habit Tracker Mini
Habit Tracker Mini adalah aplikasi Flutter sederhana untuk mencatat, menandai, dan mengelola kebiasaan harian. Aplikasi ini memuat data dari file JSON, memungkinkan pengguna menambahkan, mengedit, dan menghapus kebiasaan, serta mengganti tema terang/gelap.

# 🎯 Fitur Utama
✅ Melihat daftar kebiasaan dari file assets/habits.json.

➕ Menambahkan kebiasaan baru.

✏️ Mengedit kebiasaan yang sudah ada.

❌ Menghapus kebiasaan.

☑️ Menandai kebiasaan sebagai selesai (centang).

🔁 Reset seluruh centang dengan satu klik.

🌗 Beralih antara Dark Mode dan Light Mode.

🔢 Menampilkan progres: x/y habits.

# ✅ Pengujian Fungsional
Berikut ini checklist pengujian aplikasi:


## 🖊️ 1. Uji Strikethrough
 Centang kebiasaan → nama dan deskripsi harus dicoret.

 Batalkan centang → teks kembali normal.

🧪 Tujuan: Pastikan styling TextDecoration.lineThrough berjalan dinamis.
![WhatsApp Image 2025-06-03 at 21 52 20_c9bb141b](https://github.com/user-attachments/assets/13e1ec04-02b5-4f37-9999-7edb23788122)


## ➕ 2. Uji Tambah Habit
 Klik tombol ➕ di AppBar.

 Klik Tambah tanpa mengisi nama → harus muncul validasi “tidak boleh kosong”.

 Isi nama & deskripsi lalu simpan.

 Verifikasi: habit baru muncul di daftar.
![WhatsApp Image 2025-06-03 at 22 29 24_12601617](https://github.com/user-attachments/assets/cc550a1f-4dc2-45d0-89e0-be82226eebc9)


## ✏️ 3. Uji Edit Habit
 Klik menu tiga titik di salah satu habit.

 Pilih Edit → dialog terbuka dengan data yang sudah terisi.

 Ubah nama/deskripsi lalu Simpan.

 Perubahan langsung terlihat di daftar.
![WhatsApp Image 2025-06-03 at 21 52 38_3751523f](https://github.com/user-attachments/assets/183d673e-424c-40b3-a796-de9bdb905a22)


## 🗑️ 4. Uji Hapus Habit
 Klik tiga titik → pilih Hapus.

 Dialog konfirmasi muncul → coba tekan Batal.

 Ulangi, pilih Hapus → habit hilang dari daftar.
![WhatsApp Image 2025-06-03 at 21 51 56_6d7307ce](https://github.com/user-attachments/assets/ad377f71-b57c-4b90-b6d0-bb934f2cd750)


## 📊 5. Uji Progress Bar
 Perhatikan teks di AppBar: “Progres: x/y habits”.

 Tambahkan, centang, atau hapus habit → nilai x/y harus otomatis berubah.
![WhatsApp Image 2025-06-03 at 21 52 20_4d22897d](https://github.com/user-attachments/assets/4356e071-814a-4247-af42-cbbf77f1d034)

 
## 🔁 6. Uji Reset
 Centang beberapa habit.

 Klik tombol ⟳ di kanan bawah.

 Semua centang harus kembali kosong.

## 🧪 7. Uji Ephemeral State (Sementara)
 Tutup paksa aplikasi.

 Buka kembali.

 Semua perubahan (tambah/edit/hapus) hilang → hanya habits.json dimuat ulang.
![WhatsApp Image 2025-06-03 at 21 51 56_6819f87d](https://github.com/user-attachments/assets/8c453e16-a8f5-476c-b5d0-8051aeedfcf1)


## 🖥️ 8. Debug print Output
Perhatikan konsol ketika:

Menambahkan habit:

![WhatsApp Image 2025-06-03 at 22 38 05_a8a72c67](https://github.com/user-attachments/assets/94841f94-75d5-4389-81ba-d8e7c74518e8)
