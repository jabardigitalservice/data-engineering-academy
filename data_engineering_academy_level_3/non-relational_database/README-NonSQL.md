# **Database Non-Relasional**

![NoSQL](https://github.com/jabardigitalservice/data-engineering-academy/blob/content_temp/data_engineering_academy_level_3/non-relational_database/images/sql%20vs%20no%20sql.png)

Database Non-Relasional atau sering juga disebut dengan istilah NoSQL atau singkatan dari Not Only SQL. NoSQL ini merupakan jenis database yang tidak mengikuti struktur data tabular kolom baris pada umumnya serta tidak memerlukan skema dan relasi pada setiap tabelnya. Dengan begitu NoSQL dapat mengelola database yang skema yang lebih fleksibel dengan skalabilias yang tinggi serta query yang lebih sederhana. Struktur penyimpanan datanya pun dapat dioptimalisasikan sesuai dengan kebutuhan data yang disimpan. 

NoSQL memeliki cara sendiri untuk mengakses data tergantung pada program database yang digunakan. Selain itu NoSQL juga cukup mudah dibaca serta mudah mudah dimengerti. Dengan skalabilitas yang tinggi NoSQL juga dikatakan cocok untuk digunakan dalam mengolah data besar yang berubah-ubah seperti big data. 

Perusahaan besar seperti Google dan Facebook pun menggunakan NoSQL karena mendukung pengembangan kemampuan real-time web application. Bentuk dokumen NoSQL adalah JSON dan beberapa contoh database NoSQL yaitu Dynamo DB, Couchbase, CloudDB, MarkLogic dan yang sering digunakan yaitu MongoDB. 

## **Jenis - Jenis Sistem Database NoSQL**

NoSQL memiliki beberapa jenis sistem database yang sering digunakan pada umumnya seperti Key Value Stores, Column Stores, Document Stores, Graph Store dan juga Multi Model. Setiap jenis ini memiliki karakteristik yang berbeda dan tentunya dengan karakteristik tersebut menjadi kekuatan masing-masing jenis sistem database NoSQL. 

1. **Key Value Stores**

Salah satu jenis yang sederhana karena menyimpan database berupa pasangan Key yang bersifat unik dan Value yang dapat berupa JSON, String, BLOB atau tipe data lainnya. Jenis ini bertujuan mengelompokkan data dalam koleksi dengan catatan teridentifikasi dengan metode unique code dan memudahkan dalam menambahkan kapasitas sumber daya server. 

Penyimpanan ini memiliki memanfaatkan manfaat dari NoSQL namun dengan struktur seperti relational database. Beberapa contoh database Key Value ini seperti Redis, Riak, DynamoDB dan Memcached.

![Key Value Stores](https://github.com/jabardigitalservice/data-engineering-academy/blob/content_temp/data_engineering_academy_level_3/non-relational_database/images/con-key%20value.png)

2. **Column Stores**

Sering disebut juga dengan Wide Column seperti namanya jenis ini menyimpan data dengan bentuk kolom baris yang dinamis. Jenis ini dapat digunakan untuk query function seperti Count, AVG, SUM dan Min. 

Berbeda dengan relational database dengan jenis ini variasi lebih luas dalam cara pemberian nama dan format pada baris ataupun tabel yang sama misalnya baris tentu tidak perlu berada pada kolom yang sama selain itu juga memungkinan beberapa struktur sekaligus dengan mempertahankan fleksibilitas serta memungkinkan penyimpanan data dengan jumlah besar.

Contoh database Column Stores diantaranya yaitu Hbase, Datastax Enterprise, Apache Accumulo dan Cassandra.

![Column Stores](https://github.com/jabardigitalservice/data-engineering-academy/blob/content_temp/data_engineering_academy_level_3/non-relational_database/images/con-column.png)

3. **Document Stores**

Hampir mirip dengan Key Value namun disimpan menjadi dokumen dengan format JSON atau XML serta value tersebut dapat berupa angka, string, boolean atau arrays ataupun objek. Jenis database ini dapat digunakan untuk berbagai kasus penggunaan seperti platform blogging, aplkasi e-commerce, analisis real-time atau pun CMS. 

Dengan database document pengembang dapat menyimpan query di dalam database. Sifat dokumen ini memungkinan untuk berevolusi sesuai kebutuhan dan seiring waktu karena fleksibel dan semi-terstruktur. Beberapa database jenis document ini contohnya CouchDB, Couchbase, MongoDB, Amazon SimpleDB dan Google Firebase.

![Document Stores](https://github.com/jabardigitalservice/data-engineering-academy/blob/content_temp/data_engineering_academy_level_3/non-relational_database/images/con-document.png)

4. **Graph Stores**

Database jenis ini memiliki struktur grafik yang terdiri dari node dan edge. Dimana node tersebut terbentuk dari entitas yang menyimpan informasi mengenai orang, tempat atau hal yang berkaitan dengan entitas sedangkan edge terbentuk dari relasi antar node. 

Jenis ini digunakan dalam menemukan pola terhubung dalam data yang tidak atau pun semi terstruktur dan biasa digunakan untuk data spasial bahkan juga sering digunakan untuk mendeteksi penipuan dan juga media sosial serta mesin rekomendasi. COntoh databasenya yaitu JanusGraph, InfiniteGraph dan Neo4J.

![Graph Stores](https://github.com/jabardigitalservice/data-engineering-academy/blob/content_temp/data_engineering_academy_level_3/non-relational_database/images/con-graph.png)

5. **Multi Model**

Jenis ini merupakan gabungan dari beberapa jenis database namun juga memadukan kedua tipe database yaitu antara relational database dan non-relational. Biasanya digunakan untuk sistem yang membutuhkan lebih dari satu tipe database dalam satu waktu sekaligus contohnya seperti SQL Server, MySQL, PostgreSQL Oracle dan juga MongoDB.

## **Perbedaan NoSQL dan SQL**

| Non-Relational Database                                                       | Relational Database                                                                             |
| ------------------------------------------------------------------------------| ------------------------------------------------------------------------------------------------|
| Tidak memiliki skema tidak terstruktur (dinamis dan fleksibel)                | Memiliki skema yang tetap dan tidak dapat berubah-ubah serta harus di tentukan terlebih dahulu  |
| Sintaks atau query yang berbeda setiap jenis databasenya                      | Structured query language (SQL)                                                                 |
| Skala horizontal sehingga memudahkan dalam pengembangan                       | Cenderung skala vertikal menambah skalabilitas dengan upgrade komponen perangkat                | 
| Perkembangan komunitas begitu pesat                                           | Memiliki komunitas yang lebh besar karena lebih dulu ada dibanding NoSQL                        | 
| Cocok untuk dataset yang besar dan berubah-ubah seperti big data              | Bersifat table-based cocok untuk aplikasi transaksi multi baris                                 |
| Dirancang untuk proses analitik data semi terstruktur                         | Dirancang untuk aplikasi transaksional dan proses analisis online                               | 
| Bersifat fleksibel                                                            | Bersifat baku atau tetap                                                                        | 
| Performa tergantung pada fungsi ukuran perangkat keras dan latensi jaringan   | Performa tergantung pada struktur tabel dan query                                               | 
| Dikembangkan skala dengan arsitektur terdistribusi                            | Dikembangkan dengan meningkatkan kemampuan komputasi perangkat keras                            | 
| Memudahkan dalam menyimpan atau mengambil struktur data                       | Permintaan penyimpanan dan pengambilan dilakukan dengan query                                   | 
| Performa tergantung pada fungsi ukuran perangkat keras dan latensi jaringan   | Performa tergantung pada struktur tabel dan query                                               | 


## **Perbedaan Terminologi**
Selain perbedaan karakteristik dari NoSQL an SQL ada juga perbedaan terminologi antara setiap jenis database yang ada contohnya seperti berikut.

|SQL                    | Cassandra                    | MongoDB           |
|-----------------------| -----------------------------| ------------------|
| Table                 | Table                        | Pengumpulan       |
| Baris                 | Baris                        | Dokumen           |
| Kolom                 | Kolom                        | Bidang            | 
| Kunci Primer          | Kunci Primer                 | IdObjek           | 
| Indeks                | Indeks                       | Indeks            |     
| Tampilan              | Tampilan yang dimaterialkan  | Tampilan          | 
| Tabel / Objek Nested  | Peta                         | Dokumen Tertanam  |
| Array                 | Daftar                       | Array             |



## Referensi
https://www.niagahoster.co.id/blog/nosql-adalah/
https://www.ekrut.com/media/nosql
https://mechaid.github.io/course-materials/basis-data-lanjut/2020-2021/non-relational-database/
https://www.freepik.com/free-photos-vectors/database/2
https://www.jojonomic.com/
https://bi-insider.com/
https://bigdataanalyticsnews.com/
https://www.analyticsvidhya.com/