# **Materi Extra**

## **Mengenal Data Geospasial**
Jika data dalam definisi umumnya dapat memberikan informasi yang umum atau pun spesifik mengenai suatu seperti usia, jenis kelamin, keuangan atau alamat maka data spasial lebih fokus memberikan informasi mengenai lokasi secara rinci yang merepresentasikan objek yang ada di bumi. Informasi lokasi yang dihasilkan umumnya berdasarkan korrdinat yang didalamnya mencakup proyeksi peta dan datum. Proyeksi peta yang dimaksud tersebut adalah sistem yang mempresentasikan suatu permukaan atau bidang lengkung yang berada pada bidang datar tertentu. Sedangkan datum merupakan titik kendali dan parameter yang memiliki hubungan geometrik yang dapat dilihat melalui pengukuran atau penghitungan. Dan ada juga informasi non-spasial yaitu informasi atribut yang berkaitan dengan kondisi suatu wilayah contohnya seperti populasi penduduk, pendapatan per tahun serta jenis vegetasi dan sebagainya. 

Data spasial umumnya dibuat berdasarkan peta yang merepresentasikan objek di muka bumi beserta segala aspek yang ada di bumi baik alamiah atau buatan manusia. Informasi yang dihasilkan oleh data spasial dapat berupa titik koordinat, alamat hingga detail lokasi hingga dapat mengidentifikasi kode pos dan sebagainya. Tidak hanya itu ada beragam macam data diantaranya foot print, demographic dan consumer spending dan macam data tersebut dapat dianalisa untuk keperluan pemerintahan, publik, finansial, asuransi, utilitas listrik dan jaringan internet atau transpostasi hingga ritel dan kuliner.

## **Sumber Data Spasial**

Sumber data spasial dapat diperoleh dari hasil pengukuran baik secara langsung atau tidak langsung dari seluruh dunia. Namun sampai saat ini sumber data terbesar berasal dari Global Postioning System atau GPS dari AS. Seperti yang diketahui GPS digunakan para pengguna ponsel pintar untuk menunjukkan arah atau menemukan suatu lokasi seperti yang sering digunakan yaitu Google Maps.

Dengan GPS tersebut didapatkan posisi dengan bentuk tiga dimensi lengkap beserta informasi yang kemudian informasi spasial tersebut dipindahkan lalu disimpan dengan format yang dapat dibaca oleh perangkat lunak GIS.

Namun sumber data tidak hanya didapatkan dari GPS namun ada beberapa sumber data yang dapat digunakan diantaranya adalah:

### 1. **Peta Analog**

![Peta Analog]()

Sumber data trasional dan tertua berbentuk cetak yang dibuat dengan gulungan kertas besar dan menunjukkan data lokasi tertentu. Namun di era ini bentuk dan ukurannya sudah minimal dan mudah diakses dari ponsel pintar.

### 2. **Peta Rupa Bumi**

![Peta RBI]()

Peta yang satu ini menggambarkan macam-macam unsur pada permukaan bumi mulai dari yang alamiah hingga buatan. Indonesia memiliki peta rupa bumi yang disebut peta RBI atau peta Rupa Bumi Indonesia. Peta RBI jenis ini memiliki tujuh kategori yaitu:

* **Tema 1: Penutup Lahan**

  Menggambarkan area tutupan lahan berupa sawah, pemukiman, hutan dan sebagainya.

* **Tema 2: Hidrografi**

  Menggambarkan unsur perairan berupa pantai, danau atau sunga dan sebagainya.

* **Tema 3: Hispsografi**

  Menggambarkan ketinggian berupa kontur dan titik tinggi.

* **Tema 4: Bangunan**

  Menggambarkan bangunan berupa rumah, gedung perkantoran dan sebagainya.

* **Tema 5: Transportasi & Utilitas**

  Menggambarkan lajur kereta api dan jalan, jembatan serta kabel transmisi dan sebagainya.

* **Tema 6: Batas Administrasi**

  Menggambarkan batas wilayah seperti batas desa/kelurahan, kecamatan, kota/kabupaten, provinsi hingga batas negara.

 * **Tema 7: Toponim**

   Berisi informasi nama-nama geografi seperti nama gunung, selat, pulau dan sebagainya.

### 3. **Penginderaan Jauh**

![Penginderaan Jauh]()

Data ini dikumpulkan cara pemantauan jaraj jauh yang menggunakan teknologi berupa satelit, pesawat, drone atau kapal. Bentuk data yang dihasilkan dari penginderaan jauh ii berupa gambar raster yang nantinya dapat diolah atau dianalisis.  


## **Model Data Spasial**

Hasil data rekaman dari data spasial berkaitan dengan indikator geografis yang memiliki 2 jenis data yaitu data vektor dan data raster. Data berupa titik, garis atau poligon yang menggambarkan jalan, kota, pegunungan atau bangunan serta badan air disebut data vektor. Pada data vektor titik menggambarkan rumah, garis menggambarkan jalan dan seluruh kota digambarkan dengan poligon. Sedangkan sel piksel atau grid yang diidentifikasi berdasarkan baris dan kolom disebut dengan data raster. Citra yang dihasilkan data raster lebih kompleks layaknya citra satelit atau foto.

![Vektor Raster]()

### **Vektor**

Data spasial pada model data vektor dapat ditampilkan, disimpan dan ditempatkan berupa titik, garis atau polygon (kurva) lengkap dengan atribut. Dalam model ini juga bentuk dasar representasi data spasial disimpan sebagai koordinat kartesius x dan y. 

Kelebihan model ini adalah keakuratan representasi unsur berupa titik, garis dan polygo. Dimana dalam model vektor, garis adalah kumpulan titik yang berurut dan terhubung sedangkan polygin yang penuh dimulai dari titik awal hingga bertemu kembali dengan titik awal tersebut disimpan sebagai kumpulan daftar yang berkaitan berupa titik. 

Pada peta umumnya model data vektor ditemukan berupa jaringan sungai atau jalan dan juga berupa garis batas suatu wilayah.

![Vektor]()

### **Raster**

Data model ini didapatkan dari penginderaan jauh menggunakan satelit yang akan menghasilkan pixel element representasi dari objek geografis. Piksel tersebut akan disusun pada suatu grid atau petak dan setiap piksel tersusun akan memiliki warna berbeda yang kemudian membentuk suatu bidang. Bidang tersebut digunakan oleh data raster untuk menyimpan, menempatkan dan menampilkan data spasial. 
Model raster memiliki sifat resolution-dependent yang artunya ukuran piksel akan sangat mempengaruhi kualitas resolusi data raster. 

![Raster]()

## **Perbandingan Vektor dan Raster** 

|               |                     Vektor                            |                      Raster                                                 |
|---------------|-------------------------------------------------------|-----------------------------------------------------------------------------|
|**Kelebihan**  | + Ruang penyimpanan lebih kecil dan efisien           | + Struktur data yang sederhana                                              |
|               | + Resolusi spasial lebih tinggi                       | + Teknologi yang dibutuhkan lebih murah                                     |
|               | + Representasi sangat mendekati peta buatan manusia   | + Overlay menggunakan inderaja lebih mudah dilakukan                        |
|               | + Tranformasi koordinat dan proyeksi mudah dilakukan  | + Manipulasi dengan fungsi matematis sederhana                              |
|**Kekurangan** | - Struktur data lebih kompleks                        | - Dibutuhkan ruang penyimpanan lebih besar                                  |
|               | - Memanipulasi data lebih sulit                       | - Mentransformasi koordinat dan proyeksi lebih sulit                        |
|               | - Kebutuhan perangkat lebih mahal                     | - Representasi topologikal lebih sulit                                      |
|               | - Memerlukan waktu lebih untuk overlay bersamaan      | -                                                                           |


## **Pemrosesan Data Spasial**

Pemrosesan baik pengelolaan atau analisis data spasial bergantung pada model data. Pemrosesan tersebut berdasarkan kebutuhan dan analitik. Pemrosesan data spasial tersebut dapat dilakukan dengan beberapa teknik geoprocessing sebagai berikut.

![Pemrosesan]()



## Referensi
https://www.geoinformatika.sch.id/2017/08/mengenal-sig-dan-data-spasial#:~:text=Data%20spasial%20memiliki%20dua%20jenis%20tipe%20yaitu%20vektor%20dan%20raster.
https://www.universitas123.com/news/mengenal-lebih-jauh-tentang-apa-itu-data-geospasial-dan-fungsinya
https://ipmmojokerto.wordpress.com/2011/10/31/bakosurtanal-peta-rupa-bumi-indonesia/
https://gsuryanegara.blogspot.com/2019/10/mengenal-lebih-dalam-data-spasial-dan.html
https://www.brin.go.id/news/110263/serba-serbi-pemanfaatan-penginderaan-jauh
https://123dok.com/document/zwog4m1y-gambar-contoh-peta-analog-wibowo.html
http://www.buzzle.com/images/electronics/vector-raster-data-structure.jpg
https://geograph88.blogspot.com/2014/12/data-raster-dan-data-vektor.html
http://www.citrasatelit.com/data-raster-dan-data-vektor/
https://terralogiq.com/data-spasial-adalah/
https://www.canva.com/design