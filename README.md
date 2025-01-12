Penjelasan Proyek Pengelolaan Keuangan

Proyek ini merupakan sistem pengelolaan keuangan pribadi sederhana yang memungkinkan pengguna untuk mencatat dan menganalisis pengeluaran mereka menggunakan file CSV sebagai tempat penyimpanan data. Sistem ini dibangun dengan menggunakan Python dan memanfaatkan modul csv untuk membaca dan menulis data serta modul datetime untuk menangani format tanggal.
Fitur Utama:

    Menambah Pengeluaran: Pengguna dapat menambahkan pengeluaran baru dengan memasukkan tanggal, kategori, dan jumlah pengeluaran. Data ini kemudian disimpan dalam file CSV.

    Melihat Laporan Pengeluaran: Sistem ini memungkinkan pengguna untuk melihat laporan pengeluaran yang diringkas berdasarkan kategori. Setiap kategori menunjukkan total pengeluaran yang telah dikeluarkan untuk kategori tersebut.

    Menganalisis Pengeluaran: Sistem secara otomatis menganalisis pengeluaran yang tercatat dan mengelompokkan berdasarkan kategori, menghitung total pengeluaran untuk setiap kategori, serta menampilkan laporan yang mencakup total pengeluaran secara keseluruhan.

Penjelasan Fungsi-fungsi:

    read_expenses(file_path): Fungsi ini digunakan untuk membaca data pengeluaran dari file CSV yang ada. Setiap baris diubah menjadi dictionary dengan informasi tentang tanggal, kategori, dan jumlah pengeluaran.

    add_expense(file_path, date, category, amount): Fungsi ini digunakan untuk menambah pengeluaran baru. Data yang dimasukkan akan disimpan ke dalam file CSV. Jika file belum ada, header CSV akan ditulis terlebih dahulu.

    analyze_expenses(expenses): Fungsi ini menganalisis pengeluaran yang telah dibaca dan mengelompokkannya berdasarkan kategori. Fungsi ini menghitung total pengeluaran per kategori dan mengembalikan hasil dalam bentuk dictionary.

    show_report(summary): Fungsi ini digunakan untuk menampilkan laporan pengeluaran yang sudah dianalisis. Laporan ini menunjukkan pengeluaran berdasarkan kategori dan total pengeluaran secara keseluruhan.

Cara Penggunaan:

    Menambahkan Pengeluaran:
        Pilih menu "1. Tambah Pengeluaran".
        Masukkan tanggal pengeluaran dengan format YYYY-MM-DD.
        Masukkan kategori pengeluaran (contoh: makan, transportasi, hiburan).
        Masukkan jumlah pengeluaran dalam angka (misalnya 50000 untuk Rp50.000).

    Melihat Laporan Pengeluaran:
        Pilih menu "2. Lihat Laporan Pengeluaran" untuk melihat laporan pengeluaran berdasarkan kategori dan total pengeluaran.

    Keluar dari Sistem:
        Pilih menu "3. Keluar" untuk keluar dari sistem.

Cara Menjalankan Program:

    Pastikan Python sudah terinstall di komputer Anda.
    Pastikan file CSV (expenses.csv) berada di folder yang sama dengan skrip Python.
    Jalankan skrip menggunakan perintah:
    Buka terminal di VS Code

    Klik Terminal > New Terminal (atau tekan `Ctrl+``).

    Di terminal, pastikan Anda berada di direktori proyek yang berisi file pengelolaan_keuangan.py. Jika belum, gunakan perintah cd untuk berpindah ke folder proyek:

    cd path/to/folder/Pengelolaan_Keuangan

    Jalankan program dengan mengetikkan perintah berikut di terminal:

    python pengelolaan_keuangan.py

    Ikuti instruksi di layar untuk memilih menu dan memasukkan data pengeluaran.

Dengan menggunakan sistem ini, Anda bisa dengan mudah melacak pengeluaran bulanan, membuat anggaran, dan mengelompokkan pengeluaran untuk melihat area mana yang memerlukan perhatian lebih.
Contoh Tampilan:

=== Sistem Pengelolaan Keuangan ===
1. Tambah Pengeluaran
2. Lihat Laporan Pengeluaran
3. Keluar
Pilih menu (1/2/3): 1
Masukkan tanggal (YYYY-MM-DD): 2025-01-13
Masukkan kategori (makan, transport, hiburan, dll.): makan
Masukkan jumlah pengeluaran: 50000
Pengeluaran berhasil ditambahkan: {'date': '2025-01-13', 'category': 'makan', 'amount': 50000.0}

=== Sistem Pengelolaan Keuangan ===
1. Tambah Pengeluaran
2. Lihat Laporan Pengeluaran
3. Keluar
Pilih menu (1/2/3): 2

Laporan Pengeluaran:
- makan: Rp50,000.00
Total Pengeluaran: Rp50,000.00

Proyek ini berguna untuk membantu pengelolaan keuangan pribadi secara lebih terstruktur dan mudah. Anda dapat menyimpan catatan pengeluaran secara digital dan menganalisis pola pengeluaran Anda.
