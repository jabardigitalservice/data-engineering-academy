# **Apa itu ERD?**
Entity Relation Diagram merupakan sebuah model yang dapat mewakili logika database untuk menggambarkan hubungan antar entitas beserta atribut yang dimiliki secara detail. Dengan menggunakan ERD maka sistem database yang diancang atau dibangun dapat tergambarkan secara rapi detail serta terstruktur. Tidak hanya digunakan saat ingin membangun sistem database namun ERD juga dapat digunakan saat proses debugging  jika ditemukan adanya permasalahan pada sistem karena dengan gambaran skema database yang menggunakan ERD dapat membantu untuk menemukan dan mengatasi permasalahan yang terjadi.
 
ERD dibedakan menjadi 3 model diantaranya yaitu:
1. **Model Data Konseptual**
  Jenis model yang paling tinggi karena memuat data secara detail dan dapat digunakan untuk mendefinsikan suatu entitas data daru data referensi suatu organisasi sehingga dapat menggambarkan struktur database yang jelas entitas serta relasinya.
2. **Model Data Logis**
  Model ini lebih detail dibanding dengan Model Data Konseptual serta memiliki komponen seperti entitas operasional, transaksional dan data master. Model ini adalah pengembangan dari Model Data Konseptual sehingga data lebih rinci dan digunakan untuk informasi yang bersifa eksplisit. 
3. **Model Data Fisik**
  Model ini sering digunakan untuk perancangan database dan model ini juga merupakan pengembangan dari Model Data Logis.
 
### **Simbol-simbol ERD**

Entitas adalah sekumpulan objek yang unik dan berbeda antara satu dengan yang lainnya. Entitas ini digambarkan dengan persegi panjang.  Objek dasarnya cukup beragam, dapat berupa orang, benda informasinya dapat disimpan database. Entitas terbagi menjadi dua yaitu entitas kuat (persegi panjang atas) yang tidak bergantung pada entitas lainnya karena dapat berdiri sendiri sedangkan entitas lemah (persegi panjang bawah) bergantung pada entitas lainnya. 

![Entity](https://github.com/jabardigitalservice/data-engineering-academy/blob/content_temp/data_engineering_academy_level_3/relational_database/images/entitas.png)

Setiap entitas memiliki atribut mendeskripsikan karakteristik entitas tersebut. Atribut pun terbagi menjadi beberapa jenis diantaranya yaitu :

1. **Key Atributte**
Atribut Key berfungsi menentukan data yang penting. Biasanya berbentuk angka atau numerik. Contohnya seperti NIK atau NIM. Atribut ini disimbolkan dengan lingkaran lonjong dengan keterangan di dalamnya serta digaris bawahi.

![Key Atributte](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/atribut%20key.png)

2. **Composite Atributte**
Atribut ini memiliki beberapa bagian yang dapat dipecah. Contohnya seperti nama depan, nama tengah dan nama belakang.

![Composite Atributte](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/atribut%20composite.png)

3. **Derifative Atributte**
Atribut ini hasil dari penurunan atribut lain sehingga bergantung pada nilai atribut yang menurunkannya biasanya tidak harus ditulis atau disimpan dalam database. Contohnya selisih harga atau usia.

![Derifative Atributte](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/atribut%20derivatif.png)
 
### **Kardinalitas One to One, Many to Many dan One to Many**

Relasi yang terjadi antara 2 himpunan entitas dapat berupa Kardinalitas relasi One to One (1-1) atau Many to Many(M-N) dan juga One to Many (1-N / N-1). Kardinalitas adalah derajat yang menggambarkan jumlah maksimum entitas yang berelasi dengan entitas lain.

Pada relasi One to One (1-1) entitas A hanya boleh memiliki 1 relasi dengan 1 entitas B dan juga sebaliknya. Tidak boleh ada atribut yang sama pada kedua entitas. Contohnya 1 perusahaan mobil hanya mengeluarkan 1 merk.
 
![One to One](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/1-to-1.png)

Kebalikan dari One to One maka Many to Many memperbolehkan entitas A untuk memiliki lebih dari 1 relasi dengan entitas B dan begitu juga sebaliknya. Pada relasi ini diperbolehkan jika terdapat atribut yang sama pada kedua entitas. Contohnya banyak mahasiswa yang mengambil banyak mata kuliah.

![Many to Many](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/m-to-m.png)

One to Many (1-N) Pada setiap atribut entitas A dapat berelasi ke lebih dari 1 atribut entitas B. Contohnya seorang dokter dapat memiliki banyak pasien
 
![On to Many](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/1-to-m.png)

## **Membuat ERD**

![ERD](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/ERD.png)

ERD diatas merupakan contoh sederhana dengan mengambil sistem klinik sederhana dengan penjelasan sebagai berikut. 
 
| Entitas  | Atribut                                            |
| -------- | ---------------------------------------------------|
| Dokter   | Id Dokter, Nama Dokter, Poli                       |
| Pasien   | Id Pasien, Nama Pasien, Usia, Keluhan              |
| Obat     | Id Obat, Nama Obat, Harga Obat, Dosis, Jenis Obat  |

### **Entitas	Atribut**

Entitas dapat berupa objek, orang, benda atau informasi. Dan diatas terdapat 3 entitas yang memiliki atribut masing-masing. Lalu ada 2 relasi yaitu Rekam Medis dan Resep dimana kedua relasi tersebut juga memilki beberapa atribut. Relasi ini yang akan menghubungkan antara setiap entitasnya. Dokter akan memeriksa pasien lalu menuliskan hasilnya pada rekam medis lalu jika diperlukan maka dokter akan memberikan resep obat untuk pasien tersebut.
Entitas dokter dan entitas pasien dihubungkan dengan relasi Rekam Medis lalu antara entitas dokter dan entitas obat dihubungkan dengan relasi resep dan terakhir antara entitas pasien dan entitas obat dihubungkan dengan relasi resep. 
 
Selain itu juga terdapat kardinalitas antara setiap entitas dan relasi. Seperti pada contoh diatas yaitu setiap (1) dokter dapat mengisi banyak (M) rekam medis untuk banyak (M) pasien.  Atau jika dibalik maka setiap (1) pasien memiliki (1) rekam medis yang dibuat oleh (1) dokter yang menanganinya. Lalu (1) dokter dapat memberikan banyak (M) resep dan setiap (1) resepnya dapat terdiri dari beberapa (M) obat. Dan terakhir untuk setiap (1) pasien mendapat (1) resep dari dokter.


## Referensi

https://httpstrarask.wordpress.com/2020/01/14/contoh-kardinalitas-dan-erd/
https://www.domainesia.com/berita/pengertian-erd-adalah/
https://www.dicoding.com/blog/memahami-erd/
https://www.pinhome.id/blog/contoh-erd/
https://www.canva.com/design