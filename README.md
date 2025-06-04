# BUSGO
Tiga bagian utama yang saling berinteraksi:
Model: Mengelola data dan logika yang berhubungan dengan basis data. Ini adalah representasi tabel di database Anda.
View: Menangani logika bisnis dan memproses permintaan (request) dari pengguna.
Template: Bertanggung jawab untuk menyajikan data kepada pengguna, biasanya dalam format HTML.

Penjelasan singkat:
1. folder busgo merupakan folder Utama, file db.sqlite3 adalah database SQLite default yang digunakan Django, file manage.py berfungsi untuk menjalankan server, membuat dan menerapkan migrasi database
2. Folder busgo/bus adalah tempat di mana fungsionalitas inti terkait pengelolaan dan informasi bus (atau apapun yang menjadi fokus utama aplikasinya) diimplementasikan dan diorganisir.
- busgo/bus/migrations berfungsi untuk menyimpan "sejarah" perubahan pada struktur database Anda yang terkait dengan model-model di aplikasi.
- busgo/bus/static/bus berfungsi untuk mendefinisikan styling atau tampilan visual dari elemen-elemen HTML di halaman web.
- busgo/bus/templates/bus berisi file-file HTML (Template) yang digunakan untuk menyajikan informasi kepada pengguna.
- busgo/bus/admin.py digunakan untuk mendaftarkan Model ke dalam antarmuka administrasi bawaan Django.
- busgo/bus/models.py, Model Django, yang merepresentasikan tabel-tabel di database salah satunya Schedule (waktu keberangkatan, bus yang digunakan.
- busgo/bus/views.py merupakan tempat logika aplikasi berada. Fungsi-fungsi atau kelas-kelas di sini bertanggung jawab untuk menerima permintaan (request) dari pengguna, berinteraksi dengan Model, Melakukan pemrosesan data apa pun yang diperlukan, serta Mengirimkan data yang sudah diproses ke Template untuk ditampilkan.
4. Folder busgo/busgo secara umum adalah direktori konfigurasi utama untuk seluruh proyek.
