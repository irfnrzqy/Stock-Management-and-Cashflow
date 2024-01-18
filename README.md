# 『Deskripsi』

Program ini adalah program sederhana untuk toko serba ada (TOSERBA) yang bernama "Warung Orang Aring" dimana program ini bertujuan untuk membantu manajemen stok di Warung Orang Aring dan manajemen cashflow dari setiap pembelian yang dilakukan. Program ini merupakan program static sehingga perubahan yang terjadi ketika program ini dijalankan akan reset ketika program ini ditutup.

Pada program ini Saya menggunakan beberapa tools yang berbasis Python. Tools yang saya gunakan yaitu:

| Tools    | Versi  |                                                                                                                    Deskripsi |
| :------- | :----: | ---------------------------------------------------------------------------------------------------------------------------: |
| Python   | 3.12.0 | Python adalah bahasa yang digunakan dalam pembuatan program ini dan sudah terinstegrasi dengan library Tkinter dan datetime. |
| openpyxl | 3.1.2  |  Openpyxl adalah library Python yang berfungsi untuk mengkonversi data transaksi yang dilakukan ke dalam bentuk spreadsheet. |

# 『Fitur』

Program ini memiliki fitur-fitur yang dapat membantu pengguna dalam menggunakan program ini.

1. Informasi Barang:

   - Program ini menggunakan local dictionary ('daftar barang') yang menyimpan informasi tentang berbagai barang yang tersedia di toko. Setiap barang memiliki kode unik, nama, harga, dan jumlah stok.

2. Perhitungan Harga Barang:

   - Fungsi 'hitung harga' menghitung total harga berdasarkan kode barang ('IDbarang_input') dan jumlah barang yang dimasukkan ('jumlah_entry'). Jika pengguna membeli lebih dari 50 barang maka pengguna akan mendapatkan diskon sebesar 10%.

3. Menampilkan Informasi Barang:

   - Fungsi 'print_page' memungkinkan pengguna untuk memeriksa detail suatu barang dengan menggunakan kode uniknya. Informasi tentang detail barang akan ditampilkan di widget teks ('print_text').

4. Proses Checkout:

   - Fungsi 'checkout' memfasilitasi proses checkout. Ini memverifikasi kode barang dan jumlah, memeriksa ketersediaan stok, memberikan diskon, dan mencatat detail transaksi dalam spreadsheet('cashflow.xlsx')

5. Pencatatan Arus Kas:

   - Fungsi 'cashflow' mengelola pencatatan transaksi ke dalam spreadsheet ('cashflow.xlsx'). Ini memperbarui file yang ada atau membuat file baru bila belum ada.

# 『Cara Penggunaan』

- Install Python versi terbaru

  ```
  Download Python melalui situs resmi https://www.python.org
  ```

- Install library openpyxl di dalam terminal

  ```
  pip install openpyxl
  ```

- Jalankan program melalui terminal atau Visual Studio Code

- Masukkan kode barang di entri "kode barang"

- Klik tombol "cek stok" untuk melihat detail barang di widget teks

- Masukkan jumlah pesanan di entri "masukkan jumlah"

- Klik tombol "checkout" untuk melakukan pembelian, termasuk pembaruan stok dan pencatatan arus kas di spreadsheet.
