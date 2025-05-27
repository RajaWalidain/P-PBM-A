# Praktikum Navigasi Flutter

## 🔢 Tujuan Praktikum

Praktikum ini bertujuan untuk memahami dan mengimplementasikan berbagai jenis navigasi dalam pengembangan aplikasi Flutter, meliputi:

* Navigasi sederhana (Navigator 1.0 dengan named routes dan push)
* Navigasi versi Flutter 2.0
* Navigasi bersarang (nested navigation)
* Navigasi dengan deep linking

## 🔍 Deskripsi Aplikasi

Aplikasi yang dibangun pada praktikum ini terdiri dari empat bagian berbeda, masing-masing mendemonstrasikan jenis navigasi tertentu:

1. navigation: Menampilkan halaman utama dan beberapa layar tambahan menggunakan named route dan push.
2. navigation\_20: Menampilkan daftar item dan detailnya menggunakan struktur data yang diperluas.
3. nested\_navigation: Menampilkan proses multi-langkah (wizard) menggunakan navigator bersarang.
4. deep\_link\_navigation: Menangani rute menggunakan deep linking Flutter untuk membuka halaman tertentu secara langsung.

## 📒 Penjelasan Program

### 1. navigation

* Aplikasi dibuat menggunakan Flutter dan Dart.
* Navigasi menggunakan Navigator 1.0:

  * push() dan pushNamed().
* Terdapat daftar named route di MaterialApp.routes:

  * '/' → HomeScreen
  * '/detail' → DetailScreen
  * '/settings' → SettingsScreen
  * '/about' → AboutScreen ✅ (modifikasi)
* HomeScreen memiliki tombol menuju ke setiap screen menggunakan named route atau push langsung.
* AboutScreen menampilkan informasi deskriptif aplikasi.

### 2. navigation\_20

* Menggunakan Dart Object: Item.
* Properti Item mencakup id, name, dan description ✅ (modifikasi).
* Halaman utama menampilkan daftar item.
* Saat diklik, navigasi ke DetailScreen dan menampilkan seluruh informasi item.

### 3. nested\_navigation

* Menggunakan StatefulWidget SetupFlowScreen.
* Memanfaatkan Navigator yang memiliki key sendiri (nested).
* Tiga layar di dalam alur:

  * FindDevicesScreen
  * ConnectDeviceScreen
  * ConfirmDeviceScreen ✅ (modifikasi)
* Tiap layar menavigasi ke yang berikutnya menggunakan fungsi callback.
* ConfirmDeviceScreen menandai selesainya alur setup.

### 4. deep\_link\_navigation

* Menambahkan rute '/settings' untuk SettingsScreen ✅ (modifikasi).
* Aplikasi mampu membuka halaman SettingsScreen langsung melalui URL jika menggunakan integrasi dengan Flutter web atau URI.

## ✅ Kesimpulan

Praktikum ini memberikan pemahaman mendalam tentang berbagai pendekatan navigasi di Flutter, dari navigasi dasar hingga skenario kompleks seperti nested dan deep linking. Setiap bagian aplikasi dimodifikasi untuk mencerminkan fungsionalitas tambahan sesuai instruksi praktikum.

---

Created for Flutter Navigation Practice ✨
