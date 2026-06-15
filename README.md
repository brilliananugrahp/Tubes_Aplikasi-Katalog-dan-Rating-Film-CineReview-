Berikut adalah draf file `README.md` yang lengkap, rapi, dan siap digunakan untuk repositori GitHub proyek **CineReview** Anda.

Proyek ini merupakan aplikasi berbasis CLI (*Command Line Interface*) menggunakan bahasa pemrograman Go (Golang) untuk mengelola data koleksi film.

---

### Isi file `README.md`

```markdown
# CineReview - Aplikasi Manajemen Koleksi Film

CineReview adalah aplikasi berbasis CLI (*Command Line Interface*) yang ditulis menggunakan bahasa pemrograman **Go (Golang)**. Aplikasi ini dirancang untuk membantu pengguna mengelola, mencari, mengurutkan, dan melihat statistik dari koleksi film pribadi secara efisien dengan memanfaatkan struktur data array dan berbagai algoritma pencarian serta pengurutan.

## 🚀 Fitur Utama

Aplikasi ini dilengkapi dengan fitur CRUD (*Create, Read, Update, Delete*) serta fitur analisis data sederhana:

1. **Tambah Koleksi Film:** Memasukkan data film baru seperti Judul, Genre, Tahun Rilis, Rating (skor 0-10), dan Deskripsi Singkat.
2. **Ubah Data Film:** Memperbarui informasi film yang sudah ada berdasarkan judul tertentu.
3. **Hapus Data Film:** Menghapus film dari daftar koleksi menggunakan mekanisme *shift array*.
4. **Lihat Semua Koleksi:** Menampilkan seluruh daftar film yang tersimpan di dalam memori.
5. **Pencarian Film:**
   * **Berdasarkan Judul:** Menggunakan algoritma *Sequential Search*.
   * **Berdasarkan Genre:** Menggunakan algoritma *Binary Search (Recursive)* setelah data diurutkan.
6. **Pengurutan Koleksi Film:**
   * **Berdasarkan Rating:** Mengurutkan dari tertinggi ke terendah menggunakan *Selection Sort*.
   * **Berdasarkan Tahun Rilis:** Mengurutkan dari tahun terlama ke terbaru menggunakan *Insertion Sort*.
7. **Statistik Koleksi:** Menghitung jumlah total film per kategori genre dan menampilkan rata-rata rating dari seluruh film.

---

## 🛠️ Konsep Algoritma & Struktur Data

Untuk memenuhi aspek efisiensi, aplikasi ini menerapkan beberapa konsep fundamental ilmu komputer:

* **Struktur Data:** Array of Struct (`[NMAX]Film`) dengan alokasi statis maksimum 99 film.
* **Pencarian (Searching):**
  * *Sequential Search*: Digunakan untuk pencarian judul (karena data judul tidak diwajibkan urut).
  * *Binary Search*: Digunakan untuk pencarian genre agar proses eksekusi berjalan lebih cepat ($O(\log n)$).
* **Pengurutan (Sorting):**
  * *Insertion Sort*: Digunakan untuk pengurutan berdasarkan tahun rilis dan pengurutan genre sebelum melakukan *Binary Search*.
  * *Selection Sort*: Digunakan untuk pengurutan berdasarkan rating film.

---

## 💻 Cara Menjalankan Aplikasi

### Prasyarat
Pastikan Anda sudah menginstal **Go (Golang)** di komputer Anda. Jika belum, Anda bisa mengunduhnya di [golang.org](https://golang.org/).

### Langkah-langkah
1. **Clone Repositori ini:**
   ```bash
   git clone [https://github.com/USERNAME_ANDA/CineReview.git](https://github.com/USERNAME_ANDA/CineReview.git)
   cd CineReview

```

2. **Jalankan Aplikasi:**
Anda dapat langsung menjalankan kode tanpa melakukan *compile* terlebih dahulu dengan perintah:
```bash
go run main.go

```


3. **(Opsional) Build Aplikasi:**
Jika ingin membuat file *executable* (*binary file*):
```bash
go build main.go
./main

```



---

## 📖 Contoh Penggunaan (Preview Menu)

Ketika aplikasi dijalankan, Anda akan dihadapkan pada menu utama seperti berikut:

```text
====================================
      MENU UTAMA CINEREVIEW      
====================================
1. Tambah Koleksi Film
2. Ubah Data Film
3. Hapus Data Film
4. Lihat Semua Koleksi Film
5. Pencarian Film (Judul/Genre)
6. Urutkan Koleksi Film
7. Lihat Statistik Koleksi
0. Keluar Aplikasi
====================================
Pilih Opsi Menu (0-7): 

```

---

## 📝 Catatan Input

Aplikasi ini menggunakan fungsi kustom `BacaInput()` untuk menangani pembacaan string yang mengandung spasi agar tidak merusak antrean input *buffer* standar Go.

## 🤝 Kontribusi

Kontribusi, kritik, dan saran selalu terbuka! Silakan lakukan *fork* pada repositori ini dan buat *pull request* jika ingin menambahkan fitur baru atau memperbaiki *bug*.

```

---

### 💡 Tips untuk GitHub:
1. Pastikan Anda mengubah tautan `https://github.com/USERNAME_ANDA/CineReview.git` di atas sesuai dengan username GitHub Anda yang sebenarnya.
2. Buat file baru bernama `README.md` di direktori utama proyek Anda, lalu salin (copas) kode Markdown di atas ke dalam file tersebut.

```
