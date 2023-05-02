# **SQL**
Kependekan dari Structured Query Language merupakan bahasa baku pemrograman berorientasi himpunan (Set Oriented Language). SQL merupakan bahasa yang digunakan untuk mengakses serta mengolah database. SQL dikeluarkan sesuai standar American National Standards Institute. 
Tugas-tugas seperti pengambilan dan update adalah tugas dari SQL. Dengan SQL kita dapat membuat database dan struktur tabel, membuat query yang sederhana bahkan kompleks untuk input, update dan juga delete data dari database. Selain itu banyak sistem manajemen database relasional yang menggunakan SQL seperti Microsoft SQL Server, Oracle, Access, Ingres, Sybase dan masih banyak lagi.  

 
### **Perintah Dasar SQL**

Sebagai bahasa standar khusus untuk mengakses database relasional atau Relation Database Management System (RDBMS) perintah yang dimiliki SQL dikelompokkan menjadi beberapa kelompok umum seperti berikut: 
 
1. **DDL (Data Definition Language)**
Kelompok perintah ini berfungsi untuk mendefinisikan struktur dan skema database seperti atribut database, tabel dan kolom serta relasi antar tabel. 
 
![DDL](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/ddl.png)
 
2. **DML (Data Manipulation Language)**
Seperti namanya DML berfungsi untuk memanipulasi data dalam database seperti memasukkan dan mengambil data ke tabel, memperbarui atau menghapus data. 
 
![DML](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/dml.png)
 
3. **DCL (Data Control Language)**
Perintah DCL ini berfungsi untuk pengendalian akses data dan server database. Seperti mengatur hak apa saja yang dimiliki oleh pengguna data baik akses pada database, tabel dan field yang ada dalam database tersebut untuk keamanan dan menjaga kerahasiaan database. 
 
![DDL](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/dcl.png)

Demikian beberapa kelompok perintah SQL sesuai dengan konteksnya masing-masing, namun selain perintah di atas masih banyak perintah dasar SQL yang sering digunakan diantaranya sebagai berikut. 

![SQL Dasar](https://github.com/jabardigitalservice/data-engineering-academy/blob/content_temp/data_engineering_academy_level_3/relational_database/images/sql%20dasar.png)
___
## **Membuat View dan Datamart dengan SQL**

### **View**
Dalam SQL adalah perintah untuk membuat single table virtual yang berfungsi untuk menyimpan query SQL sederhana atau pun kompleks baik dari 1 tabel atau gabungan beberapa tabel. Dengan view dapat mempermudah dan mempercepat proses menampilkan data secara berulang serta menyembunyikan kolom tertentu yang bersifat rahasia. 

![View](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/view.png)

### **Datamart**
Merupakan subset atau dapat dikatakan sebagai bagian dari suatu data warehouse. Datamart dibangun dengan data yang terstruktur dan terpusat  karena diambil dari sumber data operasional utama sehingga fokus pada suatu subset atau suatu segmen dari data operasional yang telah dipilih serta diproses untuk tujuan tertentu seperti analisis atau laporan. 

![Datamart](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/datamart.png)
 
Datamart ini dapat dikelola secara terpisah sehingga dapat diakses serta dikelola lebih cepat dan efisien serta lebih spesifik namun datamart tetap terintegrasi dengan data warehouse. Informasi yang dihasilkan dari datamart tersebut juga akan fokus pada satu departemen atau unit bisnis di suatu organisasi dimana satu departemen atau satu unit bisnis dapat memiliki lebih dari satu datamart. 

Datamart memiliki dua arsitektur yaitu Dependent dan Independent datamart. Dependent datamart ini bersifat tersentralisasi karena dibangun dengan mengekstraksi data dari data warehouse atau dapat dikatakan bersifat terpusat karena mengambil data dari data warehouse. Sedangkan Independent data mart adalah kebalikan dari dependent karena tidak bergantung pada data dari data warehouse. Independent datamart dapat mengekstraksi data dari berbagai sumber secara langsung sehingga lebih sulit untuk dikembangkan namun cocok untuk tujuan berjangka pendek dan dapat digunakan oleh kelompok atau organisasi yang lebih kecil.
 
Berikut contoh datamart dengan menggunakan SQL. Pertama tentu membuat database lalu diikuti dengan membuat beberapa tabel untuk kebutuhan datamart. Pada contoh berikut ini terdapat tabel penjualan yang berisi data mengenai informasi penjualan, lalu ada tabel produk yang tentu berisi data mengenai produk yang di jual selain itu ada tabel tanggal yang berisi informasi mengenai detail waktu penjualan. Lalu beberapa tabel tersebut akan digabungkan dengan pemilihan data tertentu sehingga data yang didapat menjadi lebih mudah untuk dianalisis atau pun menjadi laporan. 
 
1.Membuat database
 
![Create Database](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/dm-1.png)
 
2.Membuat tabel data utama 
 
![Create Table](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/dm-2.png)
 
3.Masukkan data pada tabel utama
 
![Insert Into](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/dm-3.png)


![Table](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/dm-33.png)
 
 
4.Membuat tabel dimensi mengenai produk
 
![Insert Into](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/dm-4.png)
 
5.Masukkan data pada tabel dimensi produk
 
![Insert Into](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/m-5.png)
 

![Table](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/dm-55.png)

6.Membuat tabel dimensi mengenai waktu penjualan
 
![Create Table](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/dm-6.png)

7.Masukkan data tabel dimensi waktu penjualan
 
![Insert Into](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/dm-7.png)


![Table](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/dm-77.png)
 
 
8.Membuat datamart

![Create Datamart](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/dm-8.png)


![Table](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/dm-88.png)
___

## **SQL Advance Part 1 (Trigger)**

Trigger merupakan kode prosedural yang otomatis berjalan untuk mengeksekusi perubahan tertentu yang terjadi pada table atau tampilan database selain itu Trigger juga digunakan untuk menjaga integritas informasi. Trigger akan berjalan sebelum atau sesudah proses perintah DML yaitu Insert, Update dan Delete. 
 
![Before After](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/before%20after.png)

![Trigger](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/trigger.png)
 
Dengan keterangan sebagai berikut: 
* Create Trigger : Nama Trigger yang ingin dibuat
* {Before | After} : Waktu Trigger dijalankan
* {Insert | Update | Delete} : Trigger akan diaktifkan dengan perintah DML tersebut
* On : Mendefinisikan tabel yang akan mengaktifkan Trigger
* Begin End : Membungkus dari kode Trigger
 

## **SQL Advanced Part 2 (Fungsi dan Prosedur)**

Fungi atau function merupakan metode yang dibuat untuk menjalankan suatu perintah tertentu pada data di database. Operasi yang dijalankan dapat berupa operasi kalkulasi numerin atau non-numerik. Hampir sama dengan kawannya yaitu procedure namun function dapat mengembalikan nilai atau disebut dengan return value dan karena dapat mengembalikan nilai maka function dapat di akses seperti variabel biasa, sedangkan fungsi agregat digunakan untuk menghitung sekelompok nilai dan mengembalikan nilai tunggal atau single value.
 
Sebenarnya sudah tersedia beberapa function default dari MYSQL yang dapat digunakan seperti menghitung nilai rata-rata, menjumlahkan atau mencari nilai minimal dan maksimal. Berikut beberapa function yang akan sering digunakan yaitu:
 
1. **Count()** 

Digunakan untuk menghitung jumlah baris pada suatu tabel atau pun hanya baris dengan kondisi atau kriteria tertentu. Return value dari fungsi count ini berupa integer. 
 
![Count](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/count.png)
 
2. **Avg()**

Fungsi ini digunakan untuk menghitung rata-rata nilai suatu kolom atau record dengan suatu kriteria tertentu dengan syarat kolom tersebut adalah numerik.
 
![Avg](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/avg.png)
 
3. **Sum()**

Fungsi yang ini digunakan untuk menjumlahkan nilai suatu field atau record dengan kriteria tertentu pada kolom numerik. 
 
![Sum](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/sum.png)
 
4. **Min()**

Fungsi yang berguna untuk mencari nilai terkecil atau terendah pada suatu field numerik. 
 
![Min](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/min.png)
 
5. **Max()**

Jika fungsi min untuk mencari nilai terkecil maka max adalah untuk mencari suatu nila terbesar atau tertinggi pada suatu field. 
 
![Max](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/max.png)



## Referensi

https://www.termasmedia.com/database/mysql/416-mysql-klasifikasi-perintah-perintah-dasar-dalam-sql.html
https://www.duniailkom.com/tutorial-belajar-mysql-pengertian-view-dan-cara-penggunaan-view-dalam-mysql/
https://www.dewaweb.com/blog/sql-pengertian-fungsi-beserta-perintah-dasarnya/
https://liwato.blogspot.com/2019/05/strategi-partisi-pada-data-warehouse.html
https://kelasprogrammer.com/belajar-penggunaan-function-di-mysql/
https://chat.openai.com/c/27daecbb-1aad-4f67-8120-d3d0f1bf3c2a
https://glints.com/id/lowongan/data-mart-adalah/#.ZDtdLXZBzIV
https://ngodingdata.com/cara-membuat-trigger-mysql/
https://www.canva.com/design
https://carbon.now.sh/