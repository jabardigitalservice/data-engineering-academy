# **Database On Cloud dan On Premise**

### **On Cloud**

![On Cloud](https://github.com/jabardigitalservice/data-engineering-academy/blob/content_temp/data_engineering_academy_level_3/relational_database/images/on%20cloud.png)

Pada teknologi on cloud memungkinan iternet menjadi pusat untuk mengelola database dan juga aplikasi yang hanya bisa diakses bagi oleh pemilik hak akses. Singkatnya penyimpanan database organisasi atau perusahaan di platform cloud computing seperti Goole Cloud Platform, Amazon Wewb Services atau Microsoft Azure. Dengan teknologi cloud tidak hanya database dan aplikasi atau perangkat lunak yang dapat berbagi layanan internet namun juga server, jaringan serta penyimpanan. Layanan yang didapatkan dari cloud provider dibayar oleh pengguna secara "Pay as You Go" sehingga pengguna dapat membayar sesuai kebutuhan baik untuk meningkatkan atau menurunkan penggunaan dengan begitu maka pengguna dapat menekan biaya alih-alih membeli atau upgrade server.

Cloud Database merupakan database yang disimpan kedalam cloud untuk memudahkan konfigurasi seperti dengan 2 cara hosting cloud database yaitu IaaS atau Infrastructure as a Service atau Paas Platform as a Service. Beberapa aplikasi ini sudah menerapkan cloud database diantaranya Microsoft SQL Azure Database, Socrata dan Xeround. 

Penggunaan on cloud memiliki beberapa manfaat dan kelebihan dibanding dengan on premise karena on cloud menawarkan daya tahan serta ketersediaan yang lebih lama selain itu on cloud juga menawarkan efisiensi biaya dengan metode "Pay as You Go" serta kemudahan pemeliharaan baik dari kerusakan ataupun pencadangan.

Namun dibalik kemudahan dan efisien biaya kekurangan on cloud juga dapat menjadi pertimbangan sepeti keamaannya dan risiko terlebih jika provider hosting cloud database berbeda negara dengan pengguna. Selain itu kontrol atas performa dan konektivitas juga memerlukan jaminan jika sewaktu-waktu pengguna kehilangan kendali performa baik data atau pun fasilitas internet untuk mengakses data. 

## Jenis - Jenis Cloud Database

1. **Relational Database Service**

Pada cloud database jenis ini tersedia antarmuka SQL seperti PostgreSQL, MySQL dan SQL Server. RDS menawarkan tampilan antarmuka yang sederhana dan dapat diakses data serta aplikasi tanpa terhalang oleh masalah kompabilitas. Selain itu konfigurasi RDS juga cukup sederhana yang memduahkan sehingga tidak memakan waktu lebih untuk menyiapkannya. 

Dari segi keamanan juga dapat dikatakan kuat dan dapat ditingkatkan serta kemudahan untuk mengakses data darimana saja yang tentunya berdampak pada penghematan biaya karena RDS menawarkan harga yang terjangkau namun infrastruktur masih dapat diskalakan untuk meminimalkan pembelian perangkat keras. 

2. **MongoDB**

Jenis yang satu ini dapat digunakan secara gratis dan berbasis NoSQL sehingga dapat digunakan untuk penyimpanan data semi-terstruktur dan biasa dipakai untuk pengembangan web. Keunggulan dalam menggunakan MogoDB adalah performa yang lebih cepat dan ringan dibanding database jenis SQL. Pengelolaannya pun lebih mudah dan sederhana karena tidak memerlukan struktur tabel diawal pembuatan database sehingga pengelolaan query juga lebih baik.

Selain itu MongoDb juga dapat menampung data yang lebih bervariasi mulai dari data yang tidak terstruktur hingga data yang terstruktur karena skema tabelnya dinamis. Jika menggunakan MongoDB skalabilitas dapat sesuaikan dengan kebutuhan misalnya untuk menjalankan program yang lebih besar seperti big data. Peningkatan skalabilitas ini tentu diimbangi dengan upgrade perangkat keras dengan spesifikasi yang lebih tinggi lagi. 


3. **Firebase Realtime Database**

Jenis yang dikembangkan oleh Google dan biasa digunakan web atau aplikasi mobile yang membutuhkan kemampuan sinkronisasi data secara real-time. Firebase atau Backend as a Service (Baas) memberikan kemudahan dengan meminimalkan pekerjaan backend. Firebase menyediakan layanan gratis yaitu SPARK dan layanan berbayar yaitu BLAZE. Firebase memiliki fitur yang cukup membantu menyelesaikan pekerjaan seperti berikut:

* Firebase Analytics
* Firebase Cloud Messaging and Notifications
* Firebase Authentication
* Firebase Cloud Firestone
* Firebase Realtime Database
* Firebase Hosting
* Firebase Crashlytics
* Remote Config

4. **SimpleDB**

Jika yang tadi dikembangkan oleh Google maka jenis yang ini dikembangkan oleh Amazon Web Service dan sama seperti MongoDB karena dapat menyimpan data semi-terstruktur dengan kemudahan dalam setup dan konfigurasi namun skala yang kecil. SimpleDB menyediakan fasilitas berupa pemrosesan serta pemrosesan permintaan dan juga penyimpanan cloud selain itu juga tersedia layanan fitur yang rata-rata berbasis data tradisional. Berbeda dengan MongoDB dan Firebase jenis ini menyimpan data yang terstruktur. Namun sayangnya SimpleDB memiliki kelemahan dalam hal konsistensi dan keterbatasan penyimpanan.

5. **Big Table**

Cloud database jenis ini biasanya digunakan untuk aplikasi dengan kebutuhan skala dan kinerja yang tinggi karena satu-satunya Cloud Big Table yang dapat diskalakan menjadi ribuan kolom dengan miliaran baris sehingga dapat menyimpan terabyte dan petabyte. Dengan penyimpanan yang dikhususkan untuk data terstruktur yang berkaitan dengan pencarian internet atau operasi layanan web sehingga jenis ini menyediakan skalabilitas tinggi. 


### **On Premise**

![On Premise](https://github.com/jabardigitalservice/data-engineering-academy/blob/content_temp/data_engineering_academy_level_3/relational_database/images/on%20premise.png)

Jika on cloud database disimpan di cloud maka on premise sebaliknya database dan segala sesuatunya disimpan oleh organisasi atau perusahaan itu sendiri atau istilahnya adalah disimpan secara in-house karena organisasi aatu perusahaan tersebut yang akan mengelola seluruh infrastruktur. Metode ini dapat digunakan pada organisasi atau perusahaan yang memiliki cukup ruang untuk menyimpan perangkat infrastruktur database tersebut dan mampu mengelolanya. 
 
Sering disebut juga sebagai database tradisional dimana didalamnya terdapat sistem terstruktur antara relational database dan database warehouse yang bekerja sama pada suatu infrastuktur yang dipasang di pusat data lokal. Maka dari itu metode on premise ini membutuhkan departemen IT yang bertugas memelihara dan menjaga perangkat keras serta perangkat lunaknya dapat bekerja dengan baik.  

### **Perbedaan On Cloud dan On Premise**

![On Cloud vs On Premise](https://github.com/jabardigitalservice/data-engineering-academy/blob/content_temp/data_engineering_academy_level_3/relational_database/images/cloud%20vs%20prem.png)

|Parameter  | On Cloud                                                            | On Premise                                                                                    |
|-----------| --------------------------------------------------------------------| ----------------------------------------------------------------------------------------------|
| Sistem    | Terbagi menjadi Public, Private dan Hybrid Cloud                    | Sumber daya di deploy mandiri secara in-house                                                 |
| Kendali   | Akses data dibawah kendali prover penyedia                          | Kendali penuh oleh pengguna (organisasi atau perusahaan)                                      |
| Akses     | Dapat diakses kapanpun dan dimanapun dengan terhubung ke internet   | Kemudahan akses serta dapat memindahkan data ke server tertentu jika dibutuhkan               | 
| Keamanan  | Memungkinan combine infrastuktur data terjaga aman                  | Memudahkan dalam mengatur siapa saja yang memilki akses serta menerapkan keamanan ganda       | 
| Biaya     | Hanya membayar sesuai pemakaian (Pay as You go)                     | Semua beban biaya pengadaan perangkat keras dan perangkat lunak, server, komsumsi daya, dll   |     
| Keamanan  | Memungkinan combine infrastuktur data terjaga aman                  | Memudahkan dalam mengatur siapa saja yang memilki akses serta menerapkan keamanan ganda       | 
| Regulasi  | Memastikan kesesuaian relugasi provider                             | Mematuhi dan memastikan sisten yang dibuat sudah sesuai denga regulasi yang berlaku           |     




## Referensi

https://www.dicoding.com/blog/apa-itu-firebase-pengertian-jenis-jenis-dan-fungsi-kegunaannya/
https://sis.binus.ac.id/2023/01/06/cloud-database-vs-traditional-database/
https://www.acecloudhosting.com/blog/benefits-of-rds/
https://www.linovhr.com/cloud-database-software-hrd/
https://www.niagahoster.co.id/blog/mongodb-adalah/
https://gits.id/blog/on-premise-vs-cloud-terbaik/
https://www.whizlabs.com/blog/what-is-a-bigtable/
https://urlwebsite.com/blog/amazon-simpledb/
https://badr.co.id/id/firebase-adalah/
https://redis.com/blog/what-is-dbaas/
https://www.applixia.com/