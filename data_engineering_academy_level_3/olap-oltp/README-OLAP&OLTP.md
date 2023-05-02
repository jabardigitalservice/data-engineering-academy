# **Apa  Itu OLAP dan OLTP?**
 
## **OLAP**

Online Analytical Processing seperti namanya melakukan analisis adalah tujuan utama dari OLAP karena merupakan sebuah sistem yang digunakan untuk menganalisis multidimensi dari suatu data yang bervolume besar dan membutuhkan kecepatan yang tinggi.  Data dengan volume besar ini biasanya berasal dari data warehouse atau data mart atau pun sumber data dari penyimpanan lainnya. 

![OLAP](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/olap.png)
 
Dengan menggunakan OLAP maka menganalisis data dapat dilakukan dari beberapa database dalam waktu yang bersamaan untuk mendapatkan informasi yang lebih luas dan lebih cepat selain itu dengan OLAP juga dapat membuat prediksi sehingga OLAP sering digunakan dalam data mining, bisnis intelijen, analisis keuangan, pelaporan serta perkiraan penjualan atau anggaran. 

OLAP memiliki 3 skema dengan karakteristik masing-masing. Skema tersebut merupakan pemodelan data yang biasa digunakan untuk data dengan bentuk multidimensi. Dengan skema ini maka dapat digambarkan hubungan antara tabel fakta dengan data measures dalam aplikasi. Dan 3 jenis skema tersebut sebagai berikut:
 
1. **Star Schema** 

Skema yang paling sederhana ini menggambarkan 1 tabel fakta yang berperan sebagai tabel pusat yang dikelilingi beberapa tabel dimensi.

![Star](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/star%20sch.png)


2. **Snowflake Schema**

Pada skema ini ada beberapa tambahan beberapa tabel dimensi namun tidak secara langsung berhubungan dengan tabel fakta melainkan terhubung langsung dengan tabel dimensi lainnya.

![Snowflake](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/snowflake%20sch.png)


3. **Fact Constellation Schema/Galaxy Schema**

Berbeda dengan skema Star dan Snowflake, skema ini memiliki beberapa tabel fakta dan keduanya dapat terhubung ke tabel dimensi yang sama. 

![Fact](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/fact%20sch.png)

Setiap skema memiliki karakteristik serta kelebihan dan kekurangannya masing-masing namun setiap skema dapat digunakan sesuai dengan kebutuhan pengguna. Berikut karakteristik dimiliki setiap skema.

![Characteristic](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/111.png)

Selain itu terdapat beberapa operasi dasar OLAP yang biasa digunakan sepert penjelasan pada gambar dibawah ini.

![Operasi OLAP](https://github.com/jabardigitalservice/data-engineering-academy/blob/c6f08ec0a8fbe6a8e9f345f8bc79700a8a24ce79/data_engineering_academy_level_3/relational_database/images/Operasi%20OLAP.png)


### **Jenis - Jenis OLAP**

OLAP terbagi menjadi 3 jenis dengan cara yang berbeda dalam menyimpan data, diantaranya yaitu ROLAP (Relational On-Line Analytical Processing), MOLAP (Multidimensional On-Line Analytical Processing) dan terakhir gabungan dari keduanya yaitu HOLAP (Hybrid Online Analytical Processing). 

1. **ROLAP (Relational On-Line Analytical Processing)**

Operasi ini real time dan tidak perlu disimpan secara multidimensional karena cukup dengan menyimpannya dalam database relasional. Dengan ROLAP data berukuran besar dapat ditangani dengan cepat namun kurang dalam performa query karena tidak ada proses pre-computed data cube. 

2. **MOLAP (Multidimensional On-Line Analytical Processing)**

Kebalikan dari ROLAP dengan MOLAP penyimpanan data dilakukan dalam specialised multidimensional array structure sehingga semua elemen array dapat di definisikan namun penyimpanan data menjadi kurang efektif dan data tidak dapat disimpan secara detail. Dengan MOLAP proses query lebih sederhana serta dapat melakukan operasi OLAP seperti memanipulasi data menjadi lebih cepat namun pengguna harus melakukan refresh database dengan konsisten.

3. **HOLAP (Hybrid Online Analytical Processing)**

HOLAP dapat memudahkan dan memungkinkan menganalisis data serta mengambil keputusan dalam penyimpanan data menggunakan struktur ROLAP atau MOLAP karena HOLAP gabungan dari kedua struktur tersebut.


## **OLTP**

Online Transaction Processing ini bertujuan untuk memproses data dan data yang dimaksud adalah data transaksi sehari-hari yang biasanya memiliki arsitektur yang bertingkat. Pada kehidupan sehari-hari contoh OLTP dapat kita lihat pada transaksi ATM atau kartu kredit. Data transaksi tersebut dikelola dengan baik seperti memperbarui data, menyisipkan atau menghapus. Tidak hanya itu dengan OLTP data penting organisasi dapat terekam dengan baik seperti data manajemen, produksi, karyawan, pelanggan, pembelian atau penjualan dan masih banyak lagi. 

Penggunaan OLTP maka dapat menghemat waktu pemrosesan dan juga ruang karena dibangun dengan query yang sederhana selain itu lebih cepat serta multi akses secara langsung oleh end user. 

Pada sistem OLTP data akan dinormalisasikan dan dipecah menjadi bagian yang lebih kecil selain itu sistem OLTP dapat menjaha integritas data serta mampu memproses data transaksi yang besar dengan mandiri.

Data OLTP juga merupakan current data yang detail karena dirancang menggunakan ERD sehingga dapat memudahkan dalam pengambilan keputusan. Hasil akhir dari OLTP selain nantinya dapat membantu pengambilan keputusan namun dapat menjadi sumber data pada OLAP. 

Lalu kapan penggunaan OLTP dibutuhkan? Penggunaan OLTP dapat digunakan saat dibutuhkan proses serta penyimpanan data transaksi yang efisien dan dapat tesedia secara konsisten. 

![OLAP vs OLTP](https://github.com/jabardigitalservice/data-engineering-academy/blob/content_temp/data_engineering_academy_level_3/olap-oltp/images/olap%20vs%20oltp.png)

## **OLAP vs OLTP**

Keduanya tentu memiliki karakteristik masing-masing seperti OLAP yang diperuntukan mencari informasi sedangkan OLTP lebih fokus pada operasi atau pengelolaan. Beberapa indikator penting yang dapat memudahkan dalam mengidentifikasi OLAP serta OLTP dalam dilihat pada tabel berikut.

| Parameter          | OLAP                                                       | OLTP                                                                   |
| -------------------| -----------------------------------------------------------|------------------------------------------------------------------------|
| Karakteristik      | Mengelola data dengan jumlah besar dalam beberapa database | Mengelola data transaksi kecil dalam jumlah besar setiap harinya       |
| Tujuan             | Mencari insight untuk mendukung pengambilan keputusan      | Mendukung operasi kebutuhan organisasi secara real-time                |
| Bidang             | Indstri (Manufaktur, Travel, Keuangan, dll)                | Subjek (Pemasaran, Keuangan, Advertising, dll)                         |
| Desain Database    | Normalisasi                                                | Denormalisasi                                                          |
| Penyimpanan        | Lebih kecil (dengan pengarsipan secara berkala)            | Lebih besar                                                            |
| Query              | Sederhana                                                  | Rumit                                                                  |
| Kecepatan Respon   | Dapat merespon dalam kurun waktu milidetik (ms)            | Merespon mulai detik hingga jam sesuai dengan jumlah data              |
| Sumber Data        | Transaksi                                                  | Data OLTP, situs web, aplikasi, dll                                    |
| Target Pengguna    | Pasar                                                      | Pelanggan                                                              |
| Kapasitas Pengguna | Ribuan pengguna dalam 1 waktu sekaligus                    | Hanya beberapa pengguna dalam 1 waktu                                  |


## Referensi

http://digilib.mercubuana.ac.id/manager/t%21@file_artikel_abstrak/Isi_Artikel_185328192270.pdf
https://dosenit.com/tekno/perbedaan-oltp-vs-olap
https://lamanit.com/online-transaction-processing/
https://www.shutterstock.com/id/search/olap
https://www.complexsql.com/what-is-snowflake-schema-with-industry-examples/
https://www.geeksforgeeks.org/fact-constellation-in-data-warehouse-modelling/
https://ashutosh-bitmesra.medium.com/oltp-and-olap-what-are-the-differences-a6e21f25bfe0