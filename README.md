  1. Class Data
Tujuan: Mengelola data produk, termasuk menambahkan produk, mengambil semua data produk, dan menghitung total harga.

__init__:

Inisialisasi daftar kosong self.products untuk menyimpan data produk.
add_product:

Menambahkan produk ke dalam daftar self.products dengan atribut name (nama produk), price (harga produk), dan quantity (jumlah produk).
get_all:

Mengembalikan semua data produk yang tersimpan di self.products.
calculate_total:

Menghitung total harga semua produk berdasarkan harga dan jumlah produk.



  2. Class View
Tujuan: Mengelola tampilan dan interaksi dengan pengguna.

display_table1:

Menampilkan tabel data produk dalam format rapi dengan kolom: Produk, Harga, dan Jumlah.
display_total:

Menampilkan total harga dari semua produk.
get_input:

Mengambil input dari pengguna berdasarkan prompt yang diberikan.
display_message:

Menampilkan pesan kepada pengguna.



  3. Class Process
Tujuan: Menghubungkan data (Data) dengan tampilan (View) dan mengelola logika aplikasi.

__init__:

Menginisialisasi objek data (untuk menyimpan data produk) dan view (untuk tampilan).
add_product_data:

Meminta input dari pengguna untuk menambahkan produk baru:
Meminta nama produk, harga, dan jumlah.
Memvalidasi input (nama tidak kosong, harga dan jumlah berupa angka positif).
Menambahkan produk ke Data menggunakan add_product.
Memberikan opsi kepada pengguna apakah ingin menambahkan produk lagi.
Menangani kesalahan input dengan menampilkan pesan yang sesuai.
show_products_data:

Mengambil semua data produk dari Data dan menampilkannya menggunakan View.
Jika data produk kosong, menampilkan pesan bahwa belum ada data produk.
Menghitung dan menampilkan total harga produk.



  
4. Fungsi main

Tujuan: Fungsi utama yang menjalankan program.

Langkah-langkah:
Membuat objek Data, View, dan Process.
Menampilkan menu utama dengan tiga opsi:
1. Tambah Produk Sembako: Memanggil metode add_product_data untuk menambahkan produk.
2. Tampilkan Data Produk: Memanggil metode show_products_data untuk menampilkan data produk.
3. Keluar: Mengakhiri program.
Meminta pengguna memilih opsi dan menangani input yang tidak valid.


  5.if __name__ == "__main__":

Menentukan bahwa program hanya akan dijalankan jika file dieksekusi langsung, bukan diimpor sebagai modul.
Alur Program Program menampilkan menu utama.
Pengguna memilih opsi:
 
  
  Opsi 1: Menambahkan produk dengan input nama, harga, dan jumlah.
  
  Opsi 2: Menampilkan tabel data produk beserta total harga.
  
  Opsi 3: Keluar dari program.

Jika input pengguna tidak valid, program akan menampilkan pesan kesalahan dan meminta input ulang.
