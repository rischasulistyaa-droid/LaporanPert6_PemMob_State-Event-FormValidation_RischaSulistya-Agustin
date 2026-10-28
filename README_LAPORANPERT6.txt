Aplikasi Registrasi Filocoffe (State, Event, & Form Validation)

Aplikasi Android sederhana berbasis Jetpack Compose untuk formulir pendaftaran pelanggan baru toko kopi Filocoffe. Aplikasi ini mengimplementasikan konsep pengelolaan State, penanganan Event, serta Form Validation pada Android.

Fitur Utama
State Retention (rememberSaveable)
Menjaga data inputan form agar tidak hilang saat terjadi perubahan konfigurasi (misalnya saat rotasi layar dari Portrait ke Landscape).
Form Validation (Validasi Real-time & Submit)
Nama Lengkap: Wajib diisi dan tidak boleh kosong.
Email: Harus sesuai dengan format email yang valid (Patterns.EMAIL_ADDRESS).
Password: Minimal 8 karakter dan harus mengandung sekurang-kurangnya 1 angka.
Konfirmasi Password: Harus cocok dan sama persis dengan password.
Syarat & Ketentuan: Wajib mencentang checkbox persetujuan sebelum bisa mendaftar.
Interactive UI / Event Handling
Toggle Password Visibility: Tombol ikon mata untuk menampilkan/menyembunyikan teks password & konfirmasi password.
Reset Form: Tombol "Ulangi Pendaftaran" untuk mengosongkan kembali seluruh inputan.
Pesan Kesalahan (Error Feedback): Menampilkan pesan error spesifik jika ada inputan yang belum sesuai saat tombol daftar ditekan.
Notifikasi Keberhasilan: Menampilkan kartu ucapan selamat jika seluruh data yang diisi telah valid.
Desain Kustom (Material 3 Theme)
Menggunakan kombinasi warna khas Pink & Brown (Filocoffe Theme).
Dukungan scrollable layout agar tampilan tetap dapat diakses pada layar kecil.
 Prasyarat (Prerequisites)
Sebelum menjalankan aplikasi ini, pastikan Anda telah menginstal:
Android Studio (versi Flamingo / Giraffe / Hedgehog / versi terbaru disarankan).
JDK 11 atau yang lebih baru.
Android Emulator atau Perangkat Android Fisik dengan Android 7.0 (API Level 24) ke atas.
Cara Menjalankan Project
Metode 1: Menggunakan Android Studio (Rekomendasi)
Clone atau Download Repository
git clone https://github.com/rischasulistyaa-droid/LaporanPert6_PemMob_State-Event-FormValidation_RischaSullistya-Agustin.git


Buka Project di Android Studio
Buka Android Studio.
Pilih Open / Open an Existing Project.
Arahkan ke folder project StateEventFormValidation.
Sync Gradle
Tunggu proses Gradle Sync selesai hingga seluruh dependency berhasil diunduh.
Jalankan Aplikasi
Pilih Emulator atau Perangkat Android yang terhubung.
Klik tombol Run (Shift + F10) atau ikon panah hijau di bagian atas toolbar.
 Struktur Kode Utama
MainActivity.kt: Menampung entry point setContent dan komponen UI utama RegistrationScreen().
RegistrationScreen(): Fungsi @Composable utama yang mengatur State, logika validasi, serta susunan tata letak (Layout).
fieldColors() & ErrorText(): Komponen reusable untuk konsistensi tampilan input field dan pesan kesalahan.
