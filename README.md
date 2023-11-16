# Cheatsheet Pemrograman dengan Python
## 0. Sebelum lanjut, baca dulu!!!
### Apa isi dari buku ini??
Buku ini berisikan materi singkat dan cepat tentang konsep-konsep dasar pemrograman dengan menggunakan Python sebagai bahasa untuk memberikan contoh-contohnya. Konsep-konsep dasar yang dibahas adalah variabel, tipe data, percabangan (terdiri dari pengkondisian dan perulangan), fungsi, array dan modularisasi. Konsep-konsep dasar pemrograman ini sendiri pada dasarnya akan sama di bahasa pemrograman lainnya, sehingga ketika kalian mempelajari bahasa pemrograman lain kalian hanya perlu mempelajari sintaks baru saja. Perlu diperhatikan bahwa maksud dari buku ini hanya untuk menjelaskan konsep-konsep dasar pemrograman bukan mengenai bahasa pemrograman Python itu sendiri. Python sebagai sebuah bahasa pemrograman memiliki berbagai fitur yang dapat mempermudah penulisan program tetapi termasuk pada level yang cukup advance apabila anda baru mempelajari pemrograman.

### Kenapa contoh-contohnya menggunakan Python?
Python merupakan bahasa pemrograman yang paling populer serta sintaks mudah dibaca oleh manusia. Sehingga dengan membaca buku ini secara tidak langsung kalian juga akan mempelajari Python dan akan memberikan manfaat tambahan bagi kalian.

### Apa contoh bahasa pemrograman lain yang bisa digunakan?
C, C++, C#, Java, Kotlin, Swift, Rust, Go, dan Javascript/Typescript

### Dimana saja python bisa di pakai?
- Machine Learning / Statistik / Data analysis
- Pengembangan Web (Back-end dari Instagram dibuat dengan Python)
- Pengembangan Game
- dll (saya hanya berfokus pada 3 bidang diatas)

## 1. Hello, World
### Apa itu "Hello World"?
Hello World adalah program yang biasanya dituliskan oleh seorang programmer ketika sedang mencoba bahasa pemrograman baru. Tujuan dari program hello world adalah untuk menampilkan teks "Hello, World" pada terminal

### Bagaimana "Hello, World" ditulis dalam python?
Berikut ini merupakan "Hello, World" di dalam Python
```python
# hello_world.py
print("Hello, World")
```

## 2. Variabel
### Apa itu variabel?
Variabel merupakan cara didalam suatu program untuk menyimpan data. Data yang disimpan nantinya akan diberikan nama dan dapat digunakan dengan menyebutkan nama dari variabel tersebut.

### Dimana data disimpan?
Data akan disimpan di dalam **memory** (memory yang dimaksud disini adalah RAM)

### Bagaimana membuat variabel di dalam Python?
Variabel di dalam python dapat dibuat dengan format sebagai berikut *"nama_variabel = nilai_dari_variable"*. Nama dari suatu variabel haruslah dimulai dengan suatu huruf lalu dapat diikuti dengan huruf lainnya atau angka. Nama dari variabel tidak boleh terdiri dari simbol-simbol lain kecuali simbol**_**.

### Bagaimana contoh dari variabel pada Python??
Berikut ini merupakan contoh variabel di dalam Python
```python
# variabel.py
umur_ku = 10
umur_mu = umur_ku
print("Umur mu adalah {} sementara umurku adalah {}".format(umur_mu, umur_ku))
```

### Berikan contoh nama variabel?
Berikut ini contoh nama variabel dalam Python
```python
# variabel_2.py
inivalid = 1
ini_juga_valid = 2
variabel_valid_1  = 3
_variabel_valid_2 = 4

1_ini_tidak_valid = 1 # Python bakal error di sini
ini-bukan-variabel = 2 # Python bakal error juga di sini
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
Ya tentu saja. **Saya tidak menyarankan anda untuk lanjut membaca jawaban ini apabila anda ingin pusing**. Contohnya pada tipe data integer itu memiliki ukuran sebesar 64-bit atau 8-byte. Artinya ketika kalian membuat sebuah variabel dengan tipe data integer di dalam Python, Python akan menggunakan 8-byte dari memory/RAM komputer kalian. Dengan menggunakan 8-byte memory kalian dapat menyimpan angka dengan nilai dari -9,223,372,036,854,775,808 (-(2^63)) sampai 9,223,372,036,854,775,807 (2^63). Nilai sebesar 9 juta triliun tentunya bakal sangat jarang kalian pakai sehingga, di bahasa pemrograman lain biasanya tipe data integer memiliki berbagai variasi seperti int8 (8-bit/1-byte), int16 (16-bit/2-byte), int32 (32-bit/4-byte), dan int64 (64-bit/8-byte). Sama juga seperti float di bahasa pemrograman lain terdapat tipe data seperti float32 atau float64. Sehingga kalian bisa lebih leluasa untuk mengatur ukuran dari variabel kalian. Selain tipe-tipe data tersebut masih terdapat tipe data lain yang sifatnya bukan singular data type, tetapi compositedata type. Composite tipe data type merupakan tipe data yang tersusun dari beberapa tipe data lainnya dan akan dibahas pada tipe data lanjutan.

### Apa hubungannya dengan variable??
Seperti yang disebutkan pada part 2 bahwa variabel dapat menampung suatu data. Sekarang kita tahu bahwa terdapat berbagai data yang bisa kita tampung di dalam suatu variable contohnya
```python
nama_ku = "Eric"
umur_ku = 22
apakah_aku_laki_laki = True
apakah_aku_perempuan = False
tinggi_badan_ku = 180.15

print("nama ku adalah {}. Tipe data dari variabel nama_ku adalah {}".format(nama_ku, type(nama_ku)))
print("umur ku adalah {}. Tipe data dari variabel umur_ku adalah {}".format(umur_ku, type(umur_ku)))
print("Apakah aku laki-laki? {}. Tipe data dari variabel apakah_aku_laki_laki adalah {}".format(apakah_aku_laki_laki, type(apakah_aku_laki_laki)))
print("Apakah aku perempuan? {}. Tipe data dari variabel apakah_aku_perempuan adalah {}".format(apakah_aku_perempuan, type(apakah_aku_perempuan)))
print("Tinggi badanku adalah? {}. Tipe data dari variabel tinggi_badan_ku adalah {}".format(tinggi_badan_ku, type(tinggi_badan_ku)))
```

### Apa manfaatnya memahami tipe data??
Pemahaman mengenai tipe data sebenarnya tidak akan memiliki dampak signifikan jika kalian ingin mempelajari Python. Python itu sendiri merupakan bahasa pemrograman yang dinamis. Disebut dinamis sederhananya berarti variable di Python tidak terlalu peduli dengan tipe data dari data yang ingin kalian simpan. Berbeda dengan beberapa bahasa pemrograman lainnya seperti C/C++, C# atau Java yang merupakan bahasa pemrograman yang statis, jika kalian membuat sebuah variabel dengan tipe data integer dan setelah itu menyimpan data berupa *float*, kalian justru akan menerima error.
Contohnya
```python
# tipe_data.py
nama_ku = "Eric"
print(nama_ku)
nama_ku = 10 # Tidak akan error
print(nama_ku)
```

```c
// tipe_data.c
int x;
x = 10;
x = "Eric"; // Error
```

Hanya pada beberapa kondisi tertentu Python akan peduli pada tipe data program kalian contohnya ketika kalian ingin melakukan operasi dengan menggunakan simbol **+**. Ketika kalian menggunakan **+** pada data integer hasilnya tentu saja adalah pertambahan dari dua data atau lebih. Sementara apabila yang **+** bertemu dengan string maka hasilnya adalah berupak konkatenasi atau penggabungan dari dua string tersebut contohnya "Yogi" + "Nauval" -> "YogiNauval". Tapi ketika kalian menggunakan **+** pada data yang satunya integer dan yang lain adalah string maka justru akan menghasilkan error
```python
tipe_data_2.py
nama_1 = "Yogi"
nama_2 = "Nauval"
x = 10
print(nama_1 + " " + nama_2)
print(nama_1 + x) # Akan error karena nama_1 tipe data nya string sementara x tipe data nya integer
```

## 4. Comment
Comment adalah fitur yang umum ada di dalam berbagai bahasa pemrograman. Fitur ini memberikan kita kemampuan untuk memberikan informasi di dalam program kita. Fitur ini sudah digunakan pada contoh-contoh sebelumnya. Comment pada Python diawal dengan simbol **#**, Python nantinya akan mengacuhkan semua hal yang ada setelah **#** hingga baris berikutnya dimulai

```python
# print("Ini bakal diacuhkan oleh Python")
print("Ini bakal dijalankan oleh Python")
print("Ada comment ->") # Comment bisa juga diletakkan disini
```

