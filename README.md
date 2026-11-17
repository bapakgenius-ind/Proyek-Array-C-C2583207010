# Proyek-Array-C-C2583207010
# Sistem Monitoring Stok dan Penjualan Kantin Kampus

## Deskripsi Singkat
Proyek yang dirancang menggunakan bahasa C untuk mengelola data produk, memonitor ketersediaan stok, memproses transaksi penjualan, hingga menyajikan laporan keuangan dan statistik produk terlaris di kantin kampus secara efisien[cite: 1].

## Identitas Proyek
* **Mata Kuliah:** Algoritma dan Pemrograman Lanjutan[cite: 1]
* **Semester/Kelas:** III / PTI3A dan PTI3B[cite: 1]
* **Dosen Pengampu:** Taofik Muhammad, M.Kom[cite: 1]
* **Program Studi:** Pendidikan Teknologi Informasi, Fakultas Keguruan dan Ilmu Pendidikan, Universitas Muhammadiyah Tasikmalaya[cite: 1]

---

## Daftar Fitur Program
1. **Lihat Daftar Produk:** Menampilkan nomor, nama produk, harga satuan, dan sisa stok saat ini.
2. **Tambah Produk Baru:** Menambahkan menu/produk baru beserta validasi nama duplikat, harga, dan stok awal.
3. **Ubah Produk:** Memperbarui data harga dan stok produk berdasarkan nomor produk.
4. **Transaksi Penjualan:** Melakukan pembelian multi-produk dalam satu transaksi, menghitung subtotal, total pembayaran, serta memotong stok otomatis.
5. **Tambah Stok:** Menambahkan jumlah stok produk tertentu yang sudah terdaftar.
6. **Cari Produk:** Mencari produk berdasarkan nama (pencarian fleksibel tidak sensitif huruf besar/kecil).
7. **Urutkan Produk:** Mengurutkan daftar produk berdasarkan harga termurah atau jumlah terjual terbanyak.
8. **Laporan Penjualan:** Menampilkan rekapitulasi unit terjual, total pendapatan, serta informasi produk terlaris.
9. **Cek Stok Menipis:** Memberikan peringatan otomatis untuk produk dengan stok di bawah batas minimum (kurang dari 5).

---

## Penjelasan Penggunaan Array
Program ini memanfaatkan struktur data array satu dimensi dan dua dimensi untuk menyimpan seluruh data operasional secara terstruktur di memori utama:
* **Array 2 Dimensi (`char nama[MAX_PRODUK][PANJANG_NAMA]`):** Digunakan untuk menyimpan kumpulan nama produk (string) dengan kapasitas maksimal 50 produk[cite: 1, 2].
* **Array 1 Dimensi (`int harga[MAX_PRODUK]`, `int stok[MAX_PRODUK]`):** Menyimpan harga satuan dan sisa stok masing-masing produk berdasarkan indeks yang bersesuaian dengan array nama.
* **Array 1 Dimensi (`int terjual[MAX_PRODUK]` & `long pendapatan[MAX_PRODUK]`):** Menyimpan akumulasi jumlah unit yang berhasil terjual dan total pendapatan per produk[cite: 1, 2].
* **Variabel Pelacak (`int jumlah`):** Berfungsi untuk mencatat jumlah data aktif yang sedang tersimpan di dalam array secara dinamis hingga batas kapasitas maksimal[cite: 1, 2].

---

## Petunjuk Kompilasi dan Menjalankan Program

Pastikan komputer Anda sudah terinstal compiler C (seperti GCC). Ikuti langkah-langkah berikut di terminal/command prompt:
Buka terminal pada direktori penyimpanan file kode sumber (`.c`), lalu jalankan perintah berikut:
```bash
gcc -o kantin_kampus program.c

'''
<img>

![Screenshot 2026-11-17 214810](https://github.com/user-attachments/assets/29887519-6f2b-4ec6-991f-b3eb045f39c6)
![Screenshot 2026-11-17 214149](https://github.com/user-attachments/assets/d2aba33d-f794-4de9-8dbc-842774c7b2ab)
![Screenshot 2026-11-17 214238](https://github.com/user-attachments/assets/2a043ab2-5fa5-4119-972d-bbc13f422a13)
![Screenshot 2026-11-17 214344](https://github.com/user-attachments/assets/66a76465-fdc4-477c-a8d7-3a030346f2a0)
![Screenshot 2026-11-17 214500](https://github.com/user-attachments/assets/6d8fc134-74e8-49fa-b0dc-5a3d16143574)
![Screenshot 2026-11-17 214623](https://github.com/user-attachments/assets/1eefd88b-87df-4a97-890c-c8b21fca0050)
![Screenshot 2026-11-17 214715](https://github.com/user-attachments/assets/4f17a8a8-9506-4c46-93f5-35c67b4ab963)

![Screenshot 2026-11-17 213529](https://github.com/user-attachments/assets/66d95119-7a35-4b6b-8840-bf0fb5065486)
![Screenshot 2026-11-17 213754](https://github.com/user-attachments/assets/08f41dd8-7ceb-44dc-9d2d-9862c186270f)
![Screenshot 2026-11-17 213813](https://github.com/user-attachments/assets/aa3ba723-ee5a-4aa8-8ec9-bea3ec0199c0)
</img>
