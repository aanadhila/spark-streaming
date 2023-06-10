# SPARK

Nama   : Annisa Aulia Nadhila

Kelas  : TI - 3C

NIM  : 2041720023
#

## **Nomor 1**

1. `sys.argv`: Ini adalah daftar argumen baris perintah yang diberikan saat menjalankan program Python. `sys.argv` memungkinkan program untuk menerima input dari pengguna melalui argumen baris perintah dan mengakses nilainya.

2. `sys.stderr`: Ini adalah objek aliran standar yang digunakan untuk menampilkan pesan kesalahan atau keluaran kesalahan saat program berjalan. Biasanya digunakan untuk mencatat pesan kesalahan agar mudah dibaca dan dipahami oleh pengguna.

3. `StreamingContext`: Ini adalah kelas dalam pustaka PySpark yang digunakan untuk menginisialisasi streaming konteks untuk aplikasi streaming. StreamingContext bertindak sebagai titik masuk utama untuk mengatur aliran data dan mengatur interval pembaruan.

4. `sc`: Ini adalah objek SparkContext dalam pustaka PySpark yang mewakili koneksi ke cluster Spark. Objek ini digunakan untuk membuat RDD (Resilient Distributed Dataset) dan melakukan operasi paralel di atasnya.

5. `socketTextStream`: Ini adalah metode dalam StreamingContext yang digunakan untuk membuat aliran teks dari soket jaringan. Aliran teks ini dapat digunakan untuk mengambil data dari sumber eksternal melalui soket.

6. `reduceByKey`: Ini adalah metode dalam RDD (Resilient Distributed Dataset) PySpark yang digunakan untuk mengurangi nilai-nilai dalam pasangan kunci-nilai dengan menggunakan fungsi pengurangan. Metode ini menggabungkan nilai-nilai yang memiliki kunci yang sama.

7. `lambda line`: Ini adalah ekspresi lambda dalam Python yang digunakan untuk membuat fungsi anonim yang sederhana. Dalam konteks ini, `lambda line` menunjukkan bahwa ada parameter bernama `line` yang digunakan dalam ekspresi lambda tersebut.

8. `awaitTermination`: Ini adalah metode dalam StreamingContext yang digunakan untuk menghentikan eksekusi aplikasi streaming setelah sejumlah waktu tertentu. Metode ini memastikan bahwa program tidak berjalan selamanya dan berhenti setelah periode yang ditentukan.

## **Nomer 2**

1. `nc` : Singkatan dari "netcat", yang merupakan sebuah perangkat lunak jaringan yang digunakan untuk membaca dan menulis data melalui koneksi jaringan, baik TCP maupun UDP. Dalam konteks ini, perintah "nc" digunakan untuk menjalankan netcat.

2. `-l` : Opsi "-l" menginstruksikan netcat untuk mendengarkan (listen) pada port yang ditentukan. Dengan menggunakan opsi ini, netcat akan menjadi server yang siap menerima koneksi dari client.

3. `-k` : Opsi "-k" menginstruksikan netcat agar tetap berjalan (keep listening) setelah satu koneksi selesai. Dengan menggunakan opsi ini, netcat akan tetap mendengarkan setelah koneksi pertama selesai, sehingga dapat menerima koneksi baru dari client.

## **Nomer 3**

1. `spark-submit`: Fungsi ini digunakan untuk mengirimkan aplikasi Spark ke cluster atau menjalankannya secara lokal. Dengan menggunakan `spark-submit`, Anda dapat menentukan konfigurasi aplikasi, seperti sumber data, konfigurasi cluster, pengaturan memori, dan lain-lain. Anda dapat mengirimkan aplikasi Spark dalam bentuk file JAR atau Python.

2. `master`: Parameter ini digunakan untuk menentukan alamat atau mode manajer cluster Spark yang akan digunakan. Nilai dari `master` bisa berupa URL atau mode lokal seperti `local`, `local[4]`, atau `local[*]`. Contohnya, jika Anda menggunakan `local`, aplikasi Spark akan berjalan pada satu thread secara lokal pada mesin yang sama.

3. `local[*]`: Nilai `local[*]` digunakan untuk menjalankan aplikasi Spark secara lokal dengan menggunakan semua core yang tersedia pada mesin. Dengan menggunakan nilai ini, Spark akan secara otomatis menentukan jumlah core yang tersedia dan menggunakannya untuk pemrosesan data.

## **Nomer 4**

1. `ssc.checkpoint`: Fungsi ini digunakan dalam Apache Spark Streaming untuk mengatur titik kontrol (checkpoint) yang digunakan untuk menyimpan metadata streaming. Dengan menggunakan `ssc.checkpoint`, Anda dapat mengkonfigurasi lokasi di mana informasi status streaming disimpan untuk memulihkan keadaan aplikasi setelah kegagalan atau restart.

2. `parallelize`: Fungsi ini digunakan dalam Apache Spark untuk membuat kumpulan data terdistribusi yang disebut RDD (Resilient Distributed Dataset). Fungsi `parallelize` memungkinkan Anda mengambil koleksi data yang ada di dalam memori lokal dan mendistribusikannya secara otomatis ke dalam beberapa partisi untuk pemrosesan paralel di lingkungan Spark.

3. `updateStateByKey`: Fungsi ini digunakan dalam Apache Spark Streaming untuk mengubah dan memperbarui keadaan streaming berdasarkan kunci yang diberikan. Fungsi ini berguna untuk menghitung agregasi per-kunci dari aliran data yang diterima dari beberapa batch. Dengan `updateStateByKey`, Anda dapat menggabungkan data baru dengan keadaan yang ada untuk menghasilkan output yang diperbarui.

4. `flatMap`: Fungsi ini digunakan dalam pemrograman fungsional untuk mengaplikasikan suatu fungsi pada setiap elemen dalam suatu koleksi, dan menghasilkan keluaran dalam bentuk yang dapat di-flatten (diratakan) menjadi beberapa elemen. Dalam konteks Spark, `flatMap` adalah operasi transformasi yang dapat diterapkan pada RDD atau DataFrame untuk memecah setiap elemen menjadi nol atau lebih elemen baru, yang kemudian digunakan untuk operasi lebih lanjut seperti pemetaan (mapping) atau pengurangan (reduction).


## **Nomer 5**

1. rdd.take(5): Ini adalah sebuah operasi pada RDD (Resilient Distributed Dataset) di Apache Spark yang mengembalikan lima elemen pertama dari RDD tersebut. Fungsi ini digunakan untuk mengambil sebagian kecil data dari RDD yang digunakan untuk analisis atau pemrosesan lebih lanjut.

2. transform: Ini mungkin mengacu pada fungsi transform yang ada di Spark RDD atau DataFrame. Fungsi ini digunakan untuk menerapkan transformasi pada RDD atau DataFrame yang ada. Transformasi ini dapat berupa operasi pemetaan, filtrasi, pengurangan, dan sebagainya. Transformasi ini menghasilkan RDD atau DataFrame baru dengan hasil transformasi yang diterapkan.

3. rdd.sortByKey(False): Ini adalah sebuah operasi pada RDD di Spark yang mengurutkan elemen-elemen RDD berdasarkan kunci yang diberikan. Fungsi ini mengurutkan RDD dalam urutan menurun (descending order) berdasarkan kunci yang diberikan. Nilai parameter False menunjukkan bahwa urutan pengurutan adalah dari yang terbesar ke yang terkecil.

Masing-masing fungsi ini memiliki tujuan yang berbeda dan digunakan untuk mengoperasikan data dalam konteks pengolahan data terdistribusi menggunakan Apache Spark.