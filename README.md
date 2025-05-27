
# 🎶 Sistem Pendataan Lagu dan Penyanyi

Aplikasi berbasis C++ untuk mencatat, menyimpan, mencari, dan mengurutkan data penyanyi beserta lagu-lagunya. Proyek ini dirancang sebagai latihan pemrograman menggunakan `struct`, file handling, rekursi, dan algoritma dasar seperti sequential search dan bubble sort.

---

## 🧾 Daftar Isi

- [Fitur](#fitur)
- [Struktur Data](#struktur-data)
- [Teknologi yang Digunakan](#teknologi-yang-digunakan)
- [Struktur File](#struktur-file)
- [Cara Menjalankan](#cara-menjalankan)
- [Penjelasan Algoritma](#penjelasan-algoritma)
- [Contoh Input & Output](#contoh-input--output)

---

## ✅ Fitur

- 📝 Input data penyanyi dan lagu
- 📂 Menyimpan data secara permanen di file eksternal (`file.txt`)
- 🔁 Menampilkan seluruh lagu dengan algoritma **rekursif**
- 🔍 Mencari lagu berdasarkan nama penyanyi menggunakan **sequential search**
- 🔃 Mengurutkan lagu berdasarkan judul secara **ascending** maupun **descending** menggunakan **bubble sort**
- ❌ Keluar dari aplikasi secara bersih

---

## 🧩 Struktur Data

```cpp
struct Lagu {
    string judul, genre, durasi, tahun;
};

struct Penyanyi {
    string nama;
    Lagu lagu;
};
```

> *Catatan:* Setiap penyanyi dengan banyak lagu akan dicatat ulang sebagai entri berbeda.

---

## 💻 Teknologi yang Digunakan

| Komponen            | Deskripsi                                  |
|---------------------|---------------------------------------------|
| Bahasa Pemrograman  | C++                                         |
| Paradigma           | Procedural dengan `struct` dan fungsi       |
| Kompilator          | g++, MinGW, Dev-C++, Code::Blocks, dll      |
| Platform            | Windows / Linux                             |
| Penyimpanan Data    | File teks (`file.txt`, `count.txt`)         |
| Input/Output        | Console (CLI)                               |

---

## 📁 Struktur File

| Nama File    | Deskripsi                                         |
|--------------|---------------------------------------------------|
| `baru.cpp`   | File utama berisi semua logika program            |
| `file.txt`   | Menyimpan informasi lagu dan penyanyi             |
| `count.txt`  | Menyimpan jumlah total penyanyi yang didata       |

---

## 🚀 Cara Menjalankan

### 🔧 Kompilasi Program:
Jika menggunakan terminal atau CMD:
```bash
g++ -o lagu_app baru.cpp
./lagu_app
```

### 📱 Menu Program:
```
1. Input Data Penyanyi dan Lagu
2. Tampilkan Semua Lagu
3. Cari Lagu
4. Urutkan Lagu
5. Keluar
```

---

## 🧠 Penjelasan Algoritma

| Fitur                | Algoritma             | Deskripsi                                                                 |
|----------------------|------------------------|---------------------------------------------------------------------------|
| Menampilkan Lagu     | Rekursif               | Fungsi akan memanggil dirinya sendiri sampai akhir file tercapai         |
| Pencarian Lagu       | Sequential Search      | Mengecek data satu per satu berdasarkan nama penyanyi                    |
| Pengurutan Judul     | Bubble Sort            | Menukar data secara iteratif sampai semua lagu terurut                   |

---

## 🧪 Contoh Input & Output

### 📥 Input:
```
Masukkan jumlah penyanyi: 1
Nama Artis: BTS
Jumlah Lagu: 2
Judul Lagu: Dynamite
Genre: Pop
Durasi: 3:20
Tahun: 2020
```

### 📤 Output (Rekursif):
```
=====================================
Nama Artis  : BTS
Judul Lagu  : Dynamite
Genre Lagu  : Pop
Durasi Lagu : 3:20
Tahun Lagu  : 2020
...
```

### 🔍 Output (Search):
```
Pencarian Artis: BTS
Found:
Judul Lagu Ke-1: Dynamite
Genre Lagu Ke-1: Pop
...
```

### 🔃 Output (Sorting Ascending):
```
Urutkan lagu berdasarkan judul (Asc/Desc)? : a
Lagu setelah diurutkan:
1. Dynamite - BTS
2. Life Goes On - BTS
...
```


