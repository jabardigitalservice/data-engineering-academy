# Apa itu Relational Database?
 
![Relational Database](https://github.com/jabardigitalservice/data-engineering-academy/blob/content/data_engineering_academy_level_3/relational_database/images/relational%20db.png)
Relational Database terdiri dari kelompok item data yang disusun berbentuk baris dan kolom sehingga menjadi 1 tabel. Pada setiap barisnya menunjukkan nilai suatu objek atau informasi dan pada setiap tabel juga ditandai dengan sebuah ID atau primary key. Setiap tabel ini menyimpan informasi dan memuat data serta nilai atribut tertentu. Penyajian data relational database ini biasa digunakan untuk membuat suatu kesimpulan sebuah analisis.

 
?Mengenal tentang Primary Key dan Secondary Key
Untuk mengidentifikasi sebuah baris dalam database maka diperlukan penanda sebagai tanda pengenal yang disebut Key yang juga berfungsi untuk menghubungkan antara 1 tabel dengan tabel lainnya. 
Primary Key atau kunci utama ini menyimpan suatu nilai unik dalam database dan dapat digunakan untuk mengidentifikasi suatu baris dalam tabel. Primary Key tidak boleh berubah - ubah serta tidak boleh kosong dan harus dapat membedakan antara data lainnya dalam tabel contohnya semua orang bisa mempunyai nama yang sama namun mereka akan memiliki NIK yang berbeda maka NIK itu yang menjadi primary key.  Dapat dikatakan fungsi utama Primary key adalah sebagai pengenal.

 

Sedangkan Secondary Key atau lebih dikenal sebagai Foreign Key berfungsi untuk menghubungkan tabel. Foreign key tidak dapat mengidentifikasi sebuah baris namun dapat menerima nilai yang NULL. Atribut yang menjadi Foreign Key di tabel lain haruslah atribut yang menjadi Primary di tabel asalnya.
 

# Apa itu ERD?
Entity Relation Diagram merupakan sebuah model yang dapat mewakili logika database untuk menggambarkan hubungan antar entitas beserta atribut yang dimiliki secara detail. Dengan menggunakan ERD maka sistem database yang diancang atau dibangun dapat tergambarkan secara rapi detail serta terstruktur. Tidak hanya digunakan saat ingin membangun sistem database namun ERD juga dapat digunakan saat proses debugging  jika ditemukan adanya permasalahan pada sistem karena dengan gambaran skema database yang menggunakan ERD dapat membantu untuk menemukan dan mengatasi permasalahan yang terjadi.
 
ERD dibedakan menjadi 3 model diantaranya yaitu:
1.Model Data Konseptual 
  Jenis model yang paling tinggi karena memuat data secara detail dan dapat digunakan untuk mendefinsikan suatu entitas data daru data referensi suatu organisasi sehingga dapat menggambarkan struktur database yang jelas entitas serta relasinya.
2.Model Data Logis
  Model ini lebih detail dibanding dengan Model Data Konseptual serta memiliki komponen seperti entitas operasional, transaksional dan data master. Model ini adalah pengembangan dari Model Data Konseptual sehingga data lebih rinci dan digunakan untuk informasi yang bersifa eksplisit. 
3.Model Data Fisik
  Model ini sering digunakan untuk perancangan database dan model ini juga merupakan pengembangan dari Model Data Logis.
 
?Simbol-simbol ERD
Entitas adalah sekumpulan objek yang unik dan berbeda antara satu dengan yang lainnya. Entitas ini digambarkan dengan persegi panjang.  Objek dasarnya cukup beragam, dapat berupa orang, benda informasinya dapat disimpan database. Entitas terbagi menjadi dua yaitu entitas kuat (persegi panjang atas) yang tidak bergantung pada entitas lainnya karena dapat berdiri sendiri sedangkan entitas lemah (persegi panjang bawah) bergantung pada entitas lainnya. 
Setiap entitas memiliki atribut mendeskripsikan karakteristik entitas tersebut. Atribut pun terbagi menjadi beberapa jenis diantaranya yaitu :
1.Atribut Key
Atribut Key berfungsi menentukan data yang penting. Biasanya berbentuk angka atau numerik. Contohnya seperti NIK atau NIM. Atribut ini disimbolkan dengan lingkaran lonjong dengan keterangan di dalamnya serta digaris bawahi.
2.Atribut Composite
Atribut ini memiliki beberapa bagian yang dapat dipecah. Contohnya seperti nama depan, nama tengah dan nama belakang.
3.Atribut Derivatif
Atribut derivatif dihasilkan dari atribut lain dan tidak harus ditulis atau disimpan dalam database. Contohnya selisih harga atau usia.
 
?Kardinalitas One to One, Many to Many dan One to Many
Relasi yang terjadi antara 2 himpunan entitas dapat berupa Kardinalitas relasi One to One (1-1) atau Many to Many(M-N) dan juga One to Many (1-N / N-1). Kardinalitas adalah derajat yang menggambarkan jumlah maksimum entitas yang berelasi dengan entitas lain.

Pada relasi One to One (1-1) entitas A hanya boleh memiliki 1 relasi dengan 1 entitas B dan juga sebaliknya. Tidak boleh ada atribut yang sama pada kedua entitas. Contohnya 1 perusahaan mobil hanya mengeluarkan 1 merk.
 

Kebalikan dari One to One maka Many to Many memperbolehkan entitas A untuk memiliki lebih dari 1 relasi dengan entitas B dan begitu juga sebaliknya. Pada relasi ini diperbolehkan jika terdapat atribut yang sama pada kedua entitas. Contohnya banyak mahasiswa yang mengambil banyak mata kuliah.

One to Many (1-N) Pada setiap atribut entitas A dapat berelasi ke lebih dari 1 atribut entitas B. Contohnya seorang dokter dapat memiliki banyak pasien
 

?Membuat ERD

 
ERD diatas merupakan contoh sederhana dengan mengambil sistem klinik sederhana dengan penjelasan sebagai berikut. 
 
Entitas	Atribut
Dokter	Id Dokter, Nama Dokter, Poli
Pasien	Id Pasien, Nama Pasien, Usia, Keluhan
Obat	Id Obat, Nama Obat, Harga Obat, Dosis, Jenis Obat
 
Entitas dapat berupa objek, orang, benda atau informasi. Dan diatas terdapat 3 entitas yang memiliki atribut masing-masing. Lalu ada 2 relasi yaitu Rekam Medis dan Resep dimana kedua relasi tersebut juga memilki beberapa atribut. Relasi ini yang akan menghubungkan antara setiap entitasnya. Dokter akan memeriksa pasien lalu menuliskan hasilnya pada rekam medis lalu jika diperlukan maka dokter akan memberikan resep obat untuk pasien tersebut.
Entitas dokter dan entitas pasien dihubungkan dengan relasi Rekam Medis lalu antara entitas dokter dan entitas obat dihubungkan dengan relasi resep dan terakhir antara entitas pasien dan entitas obat dihubungkan dengan relasi resep. 
 
Selain itu juga terdapat kardinalitas antara setiap entitas dan relasi. Seperti pada contoh diatas yaitu setiap (1) dokter dapat mengisi banyak (M) rekam medis untuk banyak (M) pasien.  Atau jika dibalik maka setiap (1) pasien memiliki (1) rekam medis yang dibuat oleh (1) dokter yang menanganinya. Lalu (1) dokter dapat memberikan banyak (M) resep dan setiap (1) resep dapat terdiri dari beberapa (M) obat. Dan terakhir setiap (1) pasien mendapat (1) resep dari dokter.
#SQL
Kependekan dari Structured Query Language merupakan bahasa baku pemrograman berorientasi himpunan (Set Oriented Language). SQL merupakan bahasa yang digunakan untuk mengakses serta mengolah database. SQL dikeluarkan sesuai standar American National Standards Institute. 
Tugas-tugas seperti pengambilan dan update adalah tugas dari SQL. Dengan SQL kita dapat membuat database dan struktur tabel, membuat query yang sederhana bahkan kompleks untuk input, update dan juga delete data dari database. Selain itu banyak sistem manajemen database relasional yang menggunakan SQL seperti Microsoft SQL Server, Oracle, Access, Ingres, Sybase dan masih banyak lagi.  

 
?Apa Saja Perintah Dasar SQL
Sebagai bahasa standar khusus untuk mengakses database relasional atau Relation Database Management System (RDBMS) perintah yang dimiliki SQL dikelompokkan menjadi beberapa kelompok umum seperti berikut: 
 
1)DDL (Data Definition Language)
Kelompok perintah ini berfungsi untuk mendefinisikan struktur dan skema database seperti atribut database, tabel dan kolom serta relasi antar tabel. 
 
 
2)DML (Data Manipulation Language)
Seperti namanya DML berfungsi untuk memanipulasi data dalam database seperti memasukkan dan mengambil data ke tabel, memperbarui atau menghapus data. 
 
 
3)DCL (Data Control Language)
Perintah DCL ini berfungsi untuk pengendalian akses data dan server database. Seperti mengatur hak apa saja yang dimiliki oleh pengguna data baik akses pada database, tabel dan field yang ada dalam database tersebut untuk keamanan dan menjaga kerahasiaan database. 
 
 
Demikian beberapa kelompok perintah SQL sesuai dengan konteksnya masing-masing, namun selain perintah di atas masih banyak perintah dasar SQL yang sering digunakan diantaranya sebagai berikut. 
 
 
 
 
?Membuat View dan Datamart dengan SQL

View 
View dalam SQL adalah perintah untuk membuat single table virtual yang berfungsi untuk menyimpan query SQL sederhana atau pun kompleks baik dari 1 tabel atau gabungan beberapa tabel. Dengan view dapat mempermudah dan mempercepat proses menampilkan data secara berulang serta menyembunyikan kolom tertentu yang bersifat rahasia. 

Datamart 
Datamart merupakan subset atau dapat dikatakan sebagai bagian dari suatu data warehouse. Datamart dibangun dengan data yang terstruktur dan terpusat  karena diambil dari sumber data operasional utama sehingga fokus pada suatu subset atau suatu segmen dari data operasional yang telah dipilih serta diproses untuk tujuan tertentu seperti analisis atau laporan. 
 
Datamart ini dapat dikelola secara terpisah sehingga dapat diakses serta dikelola lebih cepat dan efisien serta lebih spesifik namun datamart tetap terintegrasi dengan data warehouse. Informasi yang dihasilkan dari datamart tersebut juga akan fokus pada satu departemen atau unit bisnis di suatu organisasi dimana satu departemen atau satu unit bisnis dapat memiliki lebih dari satu datamart. Datamart memiliki dua arsitektur yaitu Dependent dan Independent datamart. 
Dependent datamart ini bersifat tersentralisasi karena dibangun dengan mengekstraksi data dari data warehouse atau dapat dikatakan bersifat terpusat karena mengambil data dari data warehouse. Sedangkan Independent data mart adalah kebalikan dari dependent karena tidak bergantung pada data dari data warehouse. Independent datamart dapat mengekstraksi data dari berbagai sumber secara langsung sehingga lebih sulit untuk dikembangkan namun cocok untuk tujuan berjangka pendek dan dapat digunakan oleh kelompok atau organisasi yang lebih kecil.
 
Berikut contoh datamart dengan menggunakan SQL. Pertama tentu membuat database lalu diikuti dengan membuat beberapa tabel untuk kebutuhan datamart. Pada contoh berikut ini terdapat tabel penjualan yang berisi data mengenai informasi penjualan, lalu ada tabel produk yang tentu berisi data mengenai produk yang di jual selain itu ada tabel tanggal yang berisi informasi mengenai detail waktu penjualan. Lalu beberapa tabel tersebut akan digabungkan dengan pemilihan data tertentu sehingga data yang didapat menjadi lebih mudah untuk dianalisis atau pun menjadi laporan. 
 
1.Membuat database
 
 
2.Membuat tabel data utama 
 
 
3.Masukkan data pada tabel utama
 
 
 
 
4.Membuat tabel dimensi mengenai produk
 
 
5.Masukkan data pada tabel dimensi produk
 
 
 

6.Membuat tabel dimensi mengenai waktu penjualan
 
 
7.Masukkan data tabel dimensi waktu penjualan
 
 
 
 
8.Membuat datamart
 

 
 
 
?SQL Advance Part 1 (Trigger)
Trigger merupakan kode prosedural yang otomatis berjalan untuk mengeksekusi perubahan tertentu yang terjadi pada table atau tampilan database selain itu Trigger juga digunakan untuk menjaga integritas informasi. Trigger akan berjalan sebelum atau sesudah proses perintah DML yaitu Insert, Update dan Delete. 
 

 
 
 
Dengan keterangan sebagai berikut: 
?Create Trigger ��. (nama Trigger yang ingin dibuat)
?{Before | After} waktu Trigger dijalankan
?{Insert | Update | Delete} Trigger akan diaktifkan dengan perintah DML tersebut
?On mendefinisikan tabel yang akan mengaktifkan Trigger
?Begin End membungkus dari kode Trigger
 

?SQL Advanced Part 2 (Fungsi dan Prosedur)
Fungi atau function merupakan metode yang dibuat untuk menjalankan suatu perintah tertentu pada data di database. Operasi yang dijalankan dapat berupa operasi kalkulasi numerin atau non-numerik. Hampir sama dengan kawannya yaitu procedure namun function dapat mengembalikan nilai atau disebut dengan return value dan karena dapat mengembalikan nilai maka function dapat di akses seperti variabel biasa, sedangkan fungsi agregat digunakan untuk menghitung sekelompok nilai dan mengembalikan nilai tunggal atau single value.
 
Sebenarnya sudah tersedia beberapa function default dari MYSQL yang dapat digunakan seperti menghitung nilai rata-rata, menjumlahkan atau mencari nilai minimal dan maksimal.  Berikut beberapa function yang akan sering digunakan yaitu:
 
1.Count()
Digunakan untuk menghitung jumlah baris pada suatu tabel atau pun hanya baris dengan kondisi atau kriteria tertentu. Return value dari fungsi count ini berupa integer. 
 
 
2.Avg()
Fungsi ini digunakan untuk menghitung rata-rata nilai suatu kolom atau record dengan suatu kriteria tertentu dengan syarat kolom tersebut adalah numerik.
 
 
3.Sum()
Fungsi yang ini digunakan untuk menjumlahkan nilai suatu field atau record dengan kriteria tertentu pada kolom numerik. 
 
 
4.Min()
Fungsi yang berguna untuk mencari nilai terkecil atau terendah pada suatu field numerik. 
 
 
5.Max()
Jika fungsi min untuk mencari nilai terkecil maka max adalah untuk mencari suatu nila terbesar atau tertinggi pada suatu field. 
 
 
 
 
 #Apa  Itu OLAP dan OLTP?
 
?OLAP
Online Analytical Processing seperti namanya melakukan analisis adalah tujuan utama dari OLAP karena merupakan sebuah sistem yang digunakan untuk menganalisis multidimensi dari suatu data yang bervolume besar dan membutuhkan kecepatan yang tinggi.  Data dengan volume besar ini biasanya berasal dari data warehouse atau data mart atau pun sumber data dari penyimpanan lainnya. 
 
Dengan menggunakan OLAP maka menganalisis data dapat dilakukan dari beberapa database dalam waktu yang bersamaan untuk mendapatkan informasi yang lebih luas dan lebih cepat selain itu dengan OLAP juga dapat membuat prediksi sehingga OLAP sering digunakan dalam data mining, bisnis intelijen, analisis keuangan, pelaporan serta perkiraan penjualan atau anggaran. OLAP memiliki 3 skema dengan karakteristik masing-masing. Skema tersebut merupakan pemodelan data yang biasa digunakan untuk data dengan bentuk multidimensi. Dengan skema ini maka dapat digambarkan hubungan antara tabel fakta dengan data measures dalam aplikasi. Dan 3 jenis skema tersebut sebagai berikut:
 
1.Star Schema
	Skema yang paling sederhana ini menggambarkan 1 tabel fakta yang berperan sebagai tabel pusat yang dikelilingi beberapa tabel dimensi.










2.Snowflake Schema
	Pada skema ini ada beberapa tambahan beberapa tabel dimensi namun tidak secara langsung berhubungan dengan tabel fakta melainkan terhubung langsung dengan tabel dimensi lainnya.










3.Fact Constellation Schema/Galaxy Schema
	Berbeda dengan skema Star dan Snowflake, skema ini memiliki beberapa tabel fakta dan keduanya dapat terhubung ke tabel dimensi yang sama. 


Setiap skema memiliki karakteristik serta kelebihan dan kekurangannya masing-masing namun setiap skema dapat digunakan sesuai dengan kebutuhan pengguna. Berikut karakteristik dimiliki setiap skema.



Selain itu terdapat beberapa operasi dasar OLAP yang biasa digunakan sepert penjelasan pada gambar dibawah ini.


?Jenis - Jenis OLAP

OLAP terbagi menjadi 3 jenis dengan cara yang berbeda dalam menyimpan data, diantaranya yaitu ROLAP (Relational On-Line Analytical Processing), MOLAP (Multidimensional On-Line Analytical Processing) dan terakhir gabungan dari keduanya yaitu HOLAP (Hybrid Online Analytical Processing). 

1.ROLAP (Relational On-Line Analytical Processing)
Operasi ini real time dan tidak perlu disimpan secara multidimensional karena cukup dengan menyimpannya dalam database relasional. Dengan ROLAP data berukuran besar dapat ditangani dengan cepat namun kurang dalam performa query karena tidak ada proses pre-computed data cube. 

2.MOLAP (Multidimensional On-Line Analytical Processing)
Kebalikan dari ROLAP dengan MOLAP penyimpanan data dilakukan dalam specialised multidimensional array structure sehingga semua elemen array dapat di definisikan namun penyimpanan data menjadi kurang efektif dan data tidak dapat disimpan secara detail. Dengan MOLAP proses query lebih sederhana serta dapat melakukan operasi OLAP seperti memanipulasi data menjadi lebih cepat namun pengguna harus melakukan refresh database dengan konsisten.

3.HOLAP (Hybrid Online Analytical Processing)
HOLAP dapat memudahkan dan memungkinkan menganalisis data serta mengambil keputusan dalam penyimpanan data menggunakan struktur ROLAP atau MOLAP karena HOLAP gabungan dari kedua struktur tersebut.

 
? OLTP
Online Transaction Processing ini bertujuan untuk memproses data dan data yang dimaksud adalah data transaksi sehari-hari yang biasanya memiliki arsitektur yang bertingkat. Pada kehidupan sehari-hari contoh OLTP dapat kita lihat pada transaksi ATM atau kartu kredit. Data transaksi tersebut dikelola dengan baik seperti memperbarui data, menyisipkan atau menghapus. Tidak hanya itu dengan OLTP data penting organisasi dapat terekam dengan baik seperti data manajemen, produksi, karyawan, pelanggan, pembelian atau penjualan dan masih banyak lagi. 

Penggunaan OLTP maka dapat menghemat waktu pemrosesan dan juga ruang karena dibangun dengan query yang sederhana selain itu lebih cepat dan multi akses secara langsung oleh end user. Data OLTP juga merupakan current data yang detail karena dirancang menggunakan ERD sehingga dapat memudahkan dalam pengambilan keputusan Hasil akhir dari OLTP nantinya dapat membantu pengambilan keputusan serta dapat menjadi sumber data pada OLAP.
 
 
 
 
 






























Referensi
 
https://dosenit.com/kuliah-it/database/database-relasional
https://www.dicoding.com/blog/memahami-erd/
https://www.pinhome.id/blog/contoh-erd/
https://httpstrarask.wordpress.com/2020/01/14/contoh-kardinalitas-dan-erd/
https://codingstudio.id/blog/5-jenis-key-dalam-database/
https://www.termasmedia.com/database/mysql/416-mysql-klasifikasi-perintah-perintah-dasar-dalam-sql.html
https://www.dewaweb.com/blog/sql-pengertian-fungsi-beserta-perintah-dasarnya/
https://www.duniailkom.com/tutorial-belajar-mysql-pengertian-view-dan-cara-penggunaan-view-dalam-mysql/
https://ngodingdata.com/cara-membuat-trigger-mysql/
https://kelasprogrammer.com/belajar-penggunaan-function-di-mysql/
https://chat.openai.com/c/27daecbb-1aad-4f67-8120-d3d0f1bf3c2a
https://glints.com/id/lowongan/data-mart-adalah/#.ZDtdLXZBzIV
http://digilib.mercubuana.ac.id/manager/t%21@file_artikel_abstrak/Isi_Artikel_185328192270.pdf
https://www.canva.com/design
https://carbon.now.sh/
https://dosenit.com/tekno/perbedaan-oltp-vs-olap
 
 
 


