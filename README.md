# TP2DPBO2024C2

Saya Daffa Fakhry Anshori dengan NIM 2200337 mengerjakan soal TP2 dalam Praktikum mata kuliah Desain dan Pemrograman Berbasis Objek, 
untuk keberkahan-Nya maka saya tidak melakukan kecurangan seperti yang telah dispesifikasikan. Aamin. 

# Desain Program
Program yang telah dibuat adalah sebuah aplikasi Java GUI untuk manajemen data mahasiswa. Desain program ini dibangun dengan konsep objek dan menggunakan GUI Swing dari Java, memungkinkan pengguna untuk menambahkan, mengubah, dan menghapus data mahasiswa dengan mudah. Setiap operasi CRUD (Create, Read, Update, Delete) terhubung dengan database, dimana fungsi-fungsi yang melakukan operasi INSERT, SELECT, UPDATE, dan DELETE menggunakan koneksi yang disediakan oleh kelas Database. Berikut adalah desain GUI untuk program manajemen data mahasiswa:
1. Panel Utama:
   - Panel utama akan menampung semua komponen GUI, seperti formulir, tabel, dan tombol.
   - Warna latar belakang panel utama adalah putih.
2. Judul Label:
   - Label "Data Mahasiswa" akan digunakan sebagai judul utama program.
   - Judul akan memiliki ukuran teks yang lebih besar dan ditebalkan.
3. Formulir Mahasiswa:
   - Formulir akan memiliki Label dan Field untuk memasukkan NIM, Nama mahasiswa, dan ComboBox untuk memilih Jenis kelamin mahasiswa.
   - RadioButton akan digunakan untuk memilih Kelas mahasiswa.
   - Label, Field, ComboBox, dan RadioButton akan disusun secara vertikal.
4. Tabel Mahasiswa:
   - Tabel akan menampilkan data mahasiswa dalam format yang terstruktur, termasuk kolom untuk NIM, nama, jenis kelamin, dan kelas.
   - Data mahasiswa akan diambil dari database yang terhubung.
   - Pengguna dapat memilih baris tabel untuk memperbarui atau menghapus data.
5. Tombol Aksi:
   - Tombol "Add" akan menambahkan data baru ke database.
   - Tombol "Update" akan memperbarui data dalam database yang dipilih dalam tabel.
   - Tombol "Delete" akan menghapus data dalam database yang dipilih dalam tabel.
   - Tombol "Clear" akan menghapus semua input di formulir tanpa membuat perubahan pada tabel.

Untuk meningkatkan fungsionalitas aplikasi, saya telah menambahkan beberapa fitur yang dapat membantu pengguna dalam mengelola data mahasiswa dengan lebih efisien dan aman, diantaranya:
1. Penambahan prompt konfirmasi sebelum melakukan operasi delete.

   Fitur ini memastikan untuk menghindari penghapusan data yang tidak disengaja. Ketika pengguna mengklik tombol "Delete", akan muncul jendela konfirmasi dengan pesan "Hapus data?". Pengguna akan diberikan opsi untuk memilih "Yes" atau "No". Jika pengguna memilih "Yes", data mahasiswa yang dipilih akan dihapus dari database.
   
3. Validasi input sebelum operasi insert dan update.
   Fitur ini memastikan tidak ada field yang kosong sebelum menjalankan operasi INSERT atau UPDATE. Jika ada field yang kosong, pesan error akan ditampilkan.
   
5. Pengecekan duplikasi NIM sebelum operasi insert
