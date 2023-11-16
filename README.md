# Cheatsheet Pemrograman dengan Python
## 0. Sebelum lanjut, baca dulu!!!
### Apa isi dari buku ini??
Buku ini berisikan materi singkat dan cepat tentang konsep-konsep dasar pemrograman dengan menggunakan Python. Konsep-konsep dasar yang dibahas adalah variabel, tipe data, percabangan (terdiri dari pengkondisian dan perulangan), fungsi, array dan modularisasi. Konsep-konsep ini akan dijelaskan dengan menggunakan Python sebagai implementasinya. Konsep-konsep dasar pemrograman ini sendiri pada dasarnya akan sama di bahasa pemrograman lainnya, sehingga ketika anda mempelajari bahasa pemrograman lain anda hanya perlu mempelajari sintaks baru saja. Perlu diperhatikan bahwa buku ini hanya berisi konsep-konsep dasar bukan mengenai bahasa pemrograman Python itu sendiri. Python sebagai sebuah bahasa pemrograman memiliki berbagai fitur yang dapat mempermudah penulisan program tetapi termasuk pada level yang cukup advance apabila anda baru mempelajari pemrograman.

### Kenapa Python?
Python merupakan bahasa pemrograman yang paling populer serta sintaks mudah dibaca oleh manusia. Sehingga dengan memahami Python pada level dasar seharusnya buku ini sudah memberikan manfaat tambahan bagi kalian.

### Apa itu Python?
Sederhananya python adalah sebuah bahasa pemrograman dinamis yang memiliki sintaks yang mudah dibaca oleh manusia.

### Kenapa Python disebut dinamis?
(Sebaiknya kalian membaca bab mengenai variable terlebih dahulu) Python merupakan bahasa pemrograman yang variabel-nya dapat memiliki tipe data yang berubah-ubah

## 1. Hello, World
### Apa itu "Hello World"
Hello World adalah program yang biasanya dituliskan oleh seorang programmer ketika sedang mencoba bahasa pemrograman baru. Tujuan dari program hello world adalah untuk menampilkan teks "Hello, World" pada terminal

### Bagaimana "Hello, World" ditulis dalam python?
Berikut ini merupakan "Hello, World" di dalam Python
```python
# hello_world.py
print("Hello, World")
```

## 2. Variabel
### Apa itu variabel
Variabel merupakan cara didalam suatu program untuk menyimpan data. Data yang disimpan nantinya akan diberikan nama dan dapat digunakan dengan menyebutkan nama dari variabel tersebut.

### Dimana data disimpan
Data akan disimpan di dalam **memory** (memory yang dimaksud disini adalah RAM)

### Bagaimana membuat variabel di dalam Python?
Variabel di dalam python dapat dibuat dengan format sebagai berikut *"nama_variabel = nilai_dari_variable"*. Nama dari suatu variabel haruslah dimulai dengan suatu huruf lalu dapat diikuti dengan huruf lainnya atau angka. Nama dari variabel tidak boleh terdiri dari simbol-simbol lain kecuali simbol**_**.

### Berikan contoh nama variabel
Berikut ini contoh nama variabel dalam Python
```python
inivalid = 1
ini_juga_valid = 2
variabel_valid_1  = 3
_variabel_valid_2 = 4

1_ini_tidak_valid = 1
ini-bukan-variabel = 2
```

### Bagaimana contoh dari variabel pada Python??
Berikut ini merupakan contoh variabel di dalam Python
```python
# variabel.py
umur_ku = 10
umur_mu = 100
```

## 3. Tipe Data
### Apa itu tipe data??
Sebelumnya kita sudah membahas mengenai variabel. Kita sekarang mengetahui bahwa variabel adalah suatu cara untuk menyimpan **data**. Namun terdapat banyak jenis data yang sebenarnya dapat kita simpan. Pada contoh sebelumnya kita sudah menyimpan data berupa angka **10**. Tipe data dari angka **10** yang kita tuliskan itu sendiri umumnya disebut sebagai sebuah integer. Integer merupakan data-data yang merupakan angka yang tidak memiliki nilai dibelakang koma atau biasanya disebut sebagai bilangan bulat.

### Apa saja jenis-jenis tipe data??
Terdapat banyak jenis tipe data tetapi umumnya tipe data di dalam berbagai bahasa pemrograman termasuk Python akan terdiri dari
Tipe Data | Deskripsi
---------- | ----------
Integer | Data-data yang merupakan angka yang tidak memiliki nilai dibelakang koma atau disebut juga sebagai bilangan bulat
Float   | Floating point number atau angka yang memiliki nilai dibelakang koma (sebenarnya bukan koma karena metode penulisan bilangan pecahan itu menggunakan titik di dalam bahasa Inggris). Contohnya 1.0 0.5 5.1 3.14159265
String  | Merupakan tipe data yang berupa teks biasanya diawali dan diakhiri dengan tanda petik **"**
Boolean | Merupakan tipe data yang nilainya hanya terdiri dari Benar (True) atau Salah (False)

### Apakah bisa terdapat tipe data lain selain ke-4 tipe data ini?
Ya bisa saja tetapi itu akan dibahas pada tipe data lanjutan
