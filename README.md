# QuickNotes

Aplikasi ini akan menjadi aplikasi catatan sederhana dengan fitur-fitur berikut:
1.	Membuat Catatan Realtime dengan Auto Save:
o	Pengguna dapat membuat catatan dengan judul dan isi.
o	Catatan disimpan secara otomatis (auto-save) setiap kali pengguna mengetik.
2.	Todo List/Checklist:
o	Pengguna dapat menambahkan item ke dalam Todo List dengan menekan tombol +.
o	Setiap item dapat dicentang (check) atau dihapus.
3.	Fitur Tambahan:
o	Cover Gambar: Pengguna dapat menambahkan gambar sebagai cover catatan.
o	Menu Menggambar: Ikon pensil untuk membuka canvas menggambar atau corat-coret.
o	Copy All: Ikon link yang berfungsi untuk menyalin semua teks dalam catatan (dapat diubah fungsinya di masa depan).
4.	Antarmuka Pengguna:
o	Desain yang intuitif dan mudah digunakan.
o	Navigasi yang sederhana dan responsif.
________________________________________
Struktur Aplikasi
Berikut adalah gambaran struktur aplikasi yang akan dikembangkan:
1. Halaman Utama (Main Activity)
•	Menampilkan daftar semua catatan yang sudah dibuat.
•	Setiap catatan ditampilkan dalam bentuk card dengan judul, isi singkat, dan gambar cover (jika ada).
•	Tombol Buat Catatan Baru untuk membuka halaman pembuatan catatan.
2. Halaman Pembuatan/Edit Catatan (Note Activity)
•	Form Judul: Input field untuk judul catatan.
•	Form Isi: Input field untuk isi catatan.
•	Tombol +: Untuk menambahkan item ke Todo List.
•	Todo List: Daftar item yang dapat dicentang atau dihapus.
•	Menu Tambahan:
o	Ikon Gambar: Untuk menambahkan gambar sebagai cover catatan.
o	Ikon Pensil: Untuk membuka canvas menggambar.
o	Ikon Link: Untuk menyalin semua teks dalam catatan (copy all).
3. Fitur Auto Save
•	Setiap perubahan pada judul, isi, atau Todo List akan disimpan secara otomatis ke database lokal (misalnya, menggunakan Room Database).
4. Database
•	Menggunakan Room Database untuk menyimpan data catatan, Todo List, dan gambar cover.
•	Struktur tabel:
o	Note Table: ID, Judul, Isi, Gambar Cover, Tanggal Dibuat, Tanggal Diubah.
o	Todo Table: ID, ID Catatan, Item Todo, Status (centang/belum).
________________________________________
Teknologi yang Digunakan
1.	Bahasa Pemrograman: Kotlin.
2.	Tools Development: Android Studio.
3.	Database: Room Database (SQLite).
4.	UI Framework: Jetpack Compose (opsional, bisa juga menggunakan XML).
5.	Fitur Tambahan:
o	Canvas Menggambar: Menggunakan library seperti Canvas atau CustomView.
o	Image Picker: Untuk memilih gambar dari galeri atau kamera.
o	Clipboard Manager: Untuk fitur copy all.
