📱 BAGIAN 1 — Flutter Project
Setelah clone di laptop, lakukan perintah ini:

flutter pub get


Ini akan:
- Download semua dependency dari pubspec.yaml
- Bikin ulang folder .dart_tool
- Bikin ulang file build yang dibutuhkan

Kalau mau jalanin:

flutter run


👉 Tidak ada yang hilang, karena:
- lib/ ada
- assets/ ada
- pubspec.yaml ada
Itu inti project Flutter.

Folder yang tidak ikut Git seperti:

.dart_tool/
build/

→ Itu memang cuma cache & hasil compile.


🌐 BAGIAN 2 — CodeIgniter (PHP)

Setelah clone di device lain:
1️⃣ Kalau pakai Composer, lakukan perintah:

composer install

Ini bikin ulang folder:

vendor/

2️⃣ Setting database

Karena file .sql tidak ikut Git (memang tidak seharusnya):
- Import database manual ke MySQL
- Atur koneksi di:

application/config/database.php


3️⃣ Jalankan server

Kalau pakai XAMPP / Laragon:
- Taruh folder di htdocs
- Akses via browser
👉 Folder yang di-ignore seperti:

application/logs/
application/cache/


akan dibuat otomatis oleh CodeIgniter saat jalan.

❗ Kapan project BISA bermasalah setelah clone?
      Penyebab	                   Solusi
Lupa flutter pub get	      Jalankan perintahnya
Lupa composer install	      Install dependency
Database belum di-import	  Import file .sql manual
File .env tidak ada	        Buat ulang sesuai konfigurasi
