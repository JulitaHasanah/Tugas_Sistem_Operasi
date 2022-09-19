> Nama : Julita Hasanah <br>

> Nim : 2110131120005

<br><br>

<h1 align="center"><b>SISTEM OPERASI</b></h1><br>

<p align="justify">Sistem Operasi merupakan sebuah perangkat lunak yang "membungkus" perangkat keras agar lebih mudah dimanfaatkan oleh para pengguna melalui program-program aplikasi tersebut. <br><br>
Sistem Operasi bertugas untuk mengendalikan (kontrol) serta mengkoordinasikan pengunaan perangkat keras untuk berbagai program aplikasi untuk bermacam-macam pengguna.<br><br></p>

## **Komponen Sistem Operasi**

<p align="justify">Sebuah sistem operasi dapat dibagi menjadi beberapa komponen. Secara umum, para pakar sepakat bahwa terdapat sekurangnya empat komponen manajeman utama yaitu:</p>

- Manajemen Proses,
- Manajemen Memori, dan
- Manajamen Sistem Berkas.
- Manajemen Masukan/Keluaran

Selain keempat komponen di atas, Avi Silberschatz, dan kawan-kawan menambahkan beberapa komponen seperti:

- Manajemen Penyimpanan Sekunder.
- Manajemen Sistem Proteksi.
- Manajemen Jaringan.
- Command-Interpreter System.

<br>

### **Manajemen Proses**

<p align="justify">Proses adalah keadaan ketika sebuah program sedang di eksekusi. Sebuah proses membutuhkan beberapa sumber daya untuk menyelesaikan tugasnya. sumber daya tersebut dapat berupa CPU time, memori, berkas-berkas, dan perangkat-perangkat I/O. Sistem operasi bertanggung jawab atas aktivitas-aktivitas yang berkaitan dengan managemen proses seperti:</p>

- Pembuatan dan penghapusan proses pengguna dan sistem proses.
- Menunda atau melanjutkan proses.
- Menyediakan mekanisme untuk proses sinkronisasi.
- Menyediakan mekanisme untuk proses komunikasi.
- Menyediakan mekanisme untuk penanganan deadlock.

<br>

### **Manajemen Memori Utama**

<p align="justify">Memori utama atau lebih dikenal sebagai memori adalah sebuah array yang besar dari word atau byte, yang ukurannya mencapai ratusan, ribuan, atau bahkan jutaan. Setiap word atau byte mempunyai alamat tersendiri. Memori Utama berfungsi sebagai tempat penyimpanan yang akses datanya digunakan oleh CPU atau perangkat I/O. Memori utama termasuk tempat penyimpanan data yang sementara (volatile), artinya data dapat hilang begitu sistem dimatikan. Sistem operasi bertanggung jawab atas aktivitas-aktivitas yang berkaitan dengan managemen memori seperti:</p>

- Menjaga track dari memori yang sedang digunakan dan siapa yang menggunakannya.
- Memilih program yang akan di-load ke memori.
- Mengalokasikan dan meng-dealokasikan ruang memori sesuai kebutuhan.

<br>

### **Manajemen Sistem Berkas**

<p align="justify">Berkas adalah kumpulan informasi yang berhubungan sesuai dengan tujuan pembuat berkas tersebut. Berkas dapat mempunyai struktur yang bersifat hirarkis (direktori, volume, dll.). Sistem operasi bertanggung-jawab:</p>

- Pembuatan dan penghapusan berkas.
- Pembuatan dan penghapusan direktori.
- Mendukung manipulasi berkas dan direktori.
- Memetakan berkas ke secondary storage.
- Mem-backup berkas ke media penyimpanan yang permanen (non-volatile).

<br>

### **Manajemen Sistem Masukan/Keluaran**

<p align="justify">Sistem ini sering disebut dengan device manager. Menyediakan device driver yang umum sehingga operasi Masukan/Keluaran dapat seragam (membuka, membaca, menulis, menutup). Contoh: pengguna menggunakan operasi yang sama untuk membaca berkas pada perangkat keras, CD-ROM dan floppy disk. </p>

Komponen Sistem Operasi untuk sistem Masukan/Keluaran:

- Penyangga: menampung sementara data dari/ke perangkat Masukan/Keluaran.
- Spooling: melakukan penjadwalan pemakaian Masukan/Keluaran sistem supaya lebih efisien (antrian dsb.).
- Menyediakan driver: untuk dapat melakukan operasi rinci untuk perangkat keras Masukan/Keluaran tertentu.

<br>

### **Manajemen Penyimpanan Sekunder**

<p align="justify">Data yang disimpan dalam memori utama bersifat sementara dan jumlahnya sangat kecil. Oleh karena itu, untuk menyimpan keseluruhan data dan program komputer dibutuhkan penyimpanan sekunder yang bersifat permanen dan mampu menampung banyak data, sebagai back-up dari memori utama. Contoh dari penyimpanan sekunder adalah hard-disk, disket, dll. </p>

Sistem operasi bertanggung-jawab atas aktivitas-aktivitas yang berkaitan dengan manajemen disk seperti:

- free space management.
- alokasi penyimpanan.
- penjadwalan disk.

<br>

### **Sistem Proteksi**

<p align="justify">Proteksi mengacu pada mekanisme untuk mengontrol akses yang dilakukan oleh program, prosesor, atau pengguna ke sistem sumber daya. Mekanisme proteksi harus: </p>

- Membedakan antara penggunaan yang sudah diberi izin dan yang belum.
- Menspesifikasi kontrol untuk dibebankan/diberi tugas.
- Menyediakan alat untuk pemberlakuan sistem.

<br>

### **Jaringan**

<p align="justify">Sistem terdistribusi adalah sekumpulan prosesor yang tidak berbagi memori atau clock. Tiap prosesor mempunyai memori sendiri. Prosesor-prosesor tersebut terhubung melalui jaringan komunikasi Sistem terdistribusi menyediakan akses pengguna ke bermacam sumber-daya sistem. Akses tersebut menyebabkan:</p>

- Computation speed-up.
- Increased data availability.
- Enhanced reliability.

<br>

### **Command Interpreter System**

<p align="justify">Sistem Operasi menunggu instruksi dari pengguna (command driven). Program yang membaca instruksi dan mengartikan control statements umumnya disebut: control-card interpreter, command-line interpreter dan terkadang dikenal sebagai shell. 
Command-Interpreter System sangat bervariasi dari satu sistem operasi ke sistem operasi yang lain dan disesuaikan dengan tujuan dan teknologi perangkat Masukan/Keluaran yang ada. Contohnya: CLI, Windows, Pen-based (touch), dan lain-lain.</p>

<br><br>

### **Contoh Komponen Sistem operasi**

- **Manajemen Proses** <br>

  - <p align="justify">Menyediakan mekanisme untuk proses sinkronisasi. Sistem operasi akan mengatur jalanya beberapa proses yang dieksekusi bersamaan, tujuanya menghidarkan terjadinya inkonsistensi.Contohnya yaitu ketika kita membuka beberapa aplikasi tertentu pada perangkat komputer secara bersamaan dalam satu waktu maka sistem operasi akan mengatur jalanya proses agar setiap proses berjalan dengan lancar. Utuk lebih jelasnya dapat dilihat contoh penerapannya di bawah ini!<br><br>
    <img width="500px" src="gambar/1.PNG"><br>
    <img width="500px" src="gambar/2.PNG"><br>
    Untuk melihat status aplikasi/fitur yang sedang berjalan itu apa saja yaitu jika pada windows di task manager lalu pada proses, berbeda dengan linux yaitu pada terminal lalu menggunakan perintah ps atau top. Perbedaannya adalah top lebih sering digunakan secara interaktif dan ps lebih sering digunakan dalam script, digabungkan dengan perintah bash lainnya atau yang serupa. <br>
    Perintah top digunakan untuk menampilkan proses teratas yang biasanya mengkonsumsi resource sistem yang paling besar.
    <img width="500px" src="gambar/3.PNG"><br>
    <img width="500px" src="gambar/4.PNG"><br>
    <img width="500px" src="gambar/5.PNG"><br>
    pstree ini seperti pohon akar, yaitu menampilkan proses yang sedang berjalan dalam bentuk pohon.

<br>

- **Manajemen Sistem Berkas**<br>

  - Membuat folder<br>
    <img width="500px" src="gambar/6.PNG"><br>
    Untuk membuat folder menggunakan perintah mkdir _ nama folder _ . ls adalah perintah yang digunakan untuk melihat direktori pada linux.<br>

  - Membuat folder dalam folder<br>
    <img width="500px" src="gambar/7.PNG"><br>

    - Untuk menggunakan atau mengisi folder yang sudah di baut tadi amak emnggunakan perintah cd _ nama folder _
    - untuk membuat file menggunakan perintah nano _ nama file _ lalu tekan enter. Perintah nano merupakan text editor berbasis text<br>

    <img width="500px" src="gambar/8.PNG"><br>

    - Isi file txt, kemudian "ctrl+x" klik lalu klik "y" untuk menyimpan file<br>

    <img width="500px" src="gambar/9.PNG"><br>

    - Untuk mengapus file menggunakan perintah rm _ nama file _ <br>
    - Untuk mengapus folder beserta isinya menggunakan perintah rm -r _ nama folder _ <br>

<br>

- **Manajemen Masukan/Keluaran (pada linux)**
  <img width="500px" src="gambar/10.PNG"><br>
  Membuat program pada linux yaitu ketikkan pada terminal linux yaitu nano _ nama file _ .txt (ekstensi opsional)<br>
  <img width="500px" src="gambar/11.PNG"><br>
  Ketikkan isi program pada terminal. Kemudian untuk menyimpan file yaitu klik "ctrl+x" lalu ketik "y"
  <img width="500px" src="gambar/12.PNG"><br>
  Untuk melihat program yang sudah dibuat maka pada terminal ketik "cat _ namafile _ lalu klik enter. <br><br>

  <br><br>

## **Layanan Sistem Operasi**

Layanan sistem operasi dirancang untuk membuat pemrograman menjadi lebih mudah.

1. <p align="justify">Pembuatan Program: Sistem operasi menyediakan berbagai fasilitas yang membantu programer dalam membuat program seperti editor. Walaupun bukan bagian dari sistem operasi, tapi layanan ini diakses melalui sistem operasi. </p>
2. <p align="justify">Eksekusi Program: Sistem harus bisa me-load program ke memori, dan menjalankan program tersebut. Program harus bisa menghentikan pengeksekusiannya baik secara normal maupun tidak (ada error). </p>
3. <p align="justify">Operasi Masukan/Keluaran. Program yang sedang dijalankan kadang kala membutuhkan Masukan/Keluaran. Untuk efisiensi dan keamanan, pengguna biasanya tidak bisa mengatur peranti Masukan/Keluaran secara langsung, untuk itulah sistem operasi harus menyediakan mekanisme dalam melakukan operasi Masukan/Keluaran.</p>
4. <p align="justify"> Manipulasi Sistem Berkas. Program harus membaca dan menulis berkas, dan kadang kala juga harus membuat dan menghapus berkas. </p>
5. <p align="justify">komunikasi. Kadang kala sebuah proses memerlukan informasi dari proses yang lain. Ada dua cara umum dimana komunikasi dapat dilakukan. Komunikasi dapat terjadi antara proses dalam satu komputer, atau antara proses yang berada dalam komputer yang berbeda, tetapi dihubungkan oleh jaringan komputer. Komunikasi dapat dilakukan dengan share-memory atau message-passing, dimana sejumlah informasi dipindahkan antara proses oleh sistem operasi. </p>
6. <p align="justify">Deteksi Error. Sistem operasi harus selalu waspada terhadap kemungkinan error. Error dapat terjadi di CPU dan memori perangkat keras, Masukan/Keluaran, dan di dalam program yang dijalankan pengguna. Untuk setiap jenis error sistem operasi harus bisa mengambil langkah yang tepat untuk mempertahankan jalannya proses komputasi. Misalnya dengan menghentikan jalannya program, mencoba kembali melakukan operasi yang dijalankan, atau melaporkan kesalahan yang terjadi agar pengguna dapat mengambil langkah selanjutnya. </p>

<br>
Contoh :<br><br>

- **Pembuatan Program**<br>
  <img width="500px" src="gambar/terminal.PNG"><br>
  Disini saya menggunakan linux di virtual box, Untuk membuat program dan masuk ke dalam kode editor di linux menggunakan terminal, untuk itu pada layar linux klik activities lalu cari di pencarian "terminal"<br>
  <img width="500px" src="gambar/satu.PNG"><br>
  Membuat program pada linux yaitu ketikkan pada terminal linux yaitu nano _nama file_ .txt (ekstensi opsional)<br>
  <img width="500px" src="gambar/dua.PNG"><br>
  Ketikkan isi program pada terminal. Kemudian untuk menyimpan file yaitu klik "ctrl+x" lalu ketik "y"
  <img width="500px" src="gambar/tiga.png"><br>
  Untuk melihat program yang sudah dibuat maka pada terminal ketik "cat _namafile_ lalu klik enter. <br><br>

- **Operasi Masukan/Keluaran**<br>
  <img width="500px" src="gambar/empat.PNG"><br>
  operasi i/o pada linux yaitu masih pada terminal. Pada gambar di atas adalah proses output kelayar dengan menggunakan "ps" pada terinal adalah yang inputnya sendiri berasal dari system(kernel).
  <img width="500px" src="gambar/lima.PNG"><br>
  berbeda dengan gambar sebelumnya yang inputnya berasal dari system, gambar di atas adalah proses i/o yang inputnya berasar dari keyboard yaitu dengan menggunakan "cat"

  - klik cat pada terminal
  - lalu ketik inputan dari keyboard, contohnya "halo, apa kabar hari ini?"
  - stelah itu klik enter apa akan tampil output yang sama seperti yang sudah di inputkan tadi.<br>

  <img width="500px" src="gambar/enam.PNG"><br>

  - Untuk keluar dari terminal input/output ini kita bisa klik pada keyboard yaitu "ctrl+d"

<br><br>

- **Deteksi Error**<br>
  <img width="500px" src="gambar/tujuh.PNG"><br>
  Pada gambar di atas terdapat pesan error, karena mkdir kemudian outputnya tidak kita tuliskan pada perintah.

<br><br>

## **System Call**

<p align="justify">Biasanya tersedia sebagai instruksi bahasa assembly. Beberapa sistem mengizinkan system calls dibuat langsung dari program bahasa tingkat tinggi. Beberapa bahasa pemrograman (contoh: C, C++) telah didefenisikan untuk menggantikan bahasa assembly untuk sistem pemrograman. <br><br></p>

Tiga metode umum yang digunakan dalam memberikan parameter kepada sistem operasi:

- Melalui register.
- Menyimpan parameter dalam block atau tabel pada memori dan alamat block tersebut diberikan sebagai parameter dalam register.
- Menyimpan parameter (push) ke dalam stack oleh program, dan melakukan pop off pada stack oleh sistem operasi.

Contoh :

- **Membuat folder**<br>
  <img width="500px" src="gambar/delapan.PNG"><br>
  Masih di dalam terminal, untuk membuat folder pada linux maka menggunakan mkdir _ nama directori _ . ls adalah perintah yang digunakan untuk melihat direktori pada linux. Perintah ini digunakan untuk melihat atau menampilkan/list isi dari folder/direktori di linux.<br>
  <img width="500px" src="gambar/sembilan.PNG"><br>
  Jika ingin membuat beberapa folder sekaligus maka menggunakan spasi pada gambar di atas dan dapat dilihat setelah ketik perintah ls maka list direktori sudah bertambah 2 yaitu direktori tugas dan latihan.
  <img width="500px" src="gambar/sepuluh.PNG"><br>
  Namun jika ingin membuat foder dengan suku kata lebih dari satu bisa menggunakan "\"untuk pemisahnya seperti pada gambar di atas.

<br>

- **Membuat file**<br>
  <img width="500px" src="gambar/sebelas.PNG"><br>

  - Disini saya akan memgisi folder test yang sudah dibuat tadi maka untuk membuka folder tersebut menggunakan "cd _ nama folder _" dapat dilihat dengan ls folder masih kosong. <br>
  - Perintah touch _ nama file_ adalah perintah untuk membuat file baru yang kosong.
  - Perintah cat berfungsi untuk menampilkan isi dari file, daat terliat file masih kosong karena belum diisi apapun.<br>

  <img width="500px" src="gambar/duabelas.PNG"><br>

  - Jika kita ingin membuat file beserta dengan isinya pada terminal menggunakan nano _ nama file _ lalu tekan enter. nano merupakan text editor berbasis text.<br>

  <img width="500px" src="gambar/tigabelas.PNG"><br>

  - Isi file txt, kemudian "ctrl+x" klik lalu klik "y" untuk menyimpan file

  <img width="500px" src="gambar/empatbelas.PNG"><br>
  Untuk melihat isi folder test ketik "ls" maka dapat dilihat bahwa isi folder sudah terdapat dua file yaitu file1.txt dan file2.txt <br>
  cat file1.txt berfungsi untuk melihat isi dari file1.txt dapat dilihat bahwa isi dari file tersebut kosong.<br>
  cat file2.txt berfungsi untuk melihat isi dari file tersebut, dapat dilihat bahwa isinya "Belajar membuat file di..."

  <br>

- **Menghapus file dan folder**<br>

  - Menghapus file<br>
    <img width="500px" src="gambar/limabelas.PNG"><br>
    Untuk menghapus file maka menggunakan perintah rm _ nama file _ seperti pada gambar di atas yaitu rm file1.txt<br>
    Untuk melihat isi dari folder test dapat menggunakan perintah ls, dapat dilihat bahwa file1.txt sudah terhapus dari folder text<br>

  - Menghapus folder<br>
    <img width="500px" src="gambar/enambelas.PNG"><br>
    Masih di dalam folder test, di dalam folder ini saya buat lagi folder bernama latihan, di dalam latihan saya buat file bernama latihan1.txt <br>
    Kemudian untuk menghapus folder latihan beserta isi yag ada didalamnya maka menggunakan perintah rm -r _ nama folder _ . Dapat dilihat dengan peintah ls bahwa folder latihan sudah terhapus dan tidak ada lagi di folder test. <br><br>

> Keterangan : <br>
> Sebenarnya file tugas 3 ini sudah dikirim tepat waktu sebelum deadline, tetapi karna ada kesalahan saat mengirim file tugas 3 maka semua file yang ada pada origin master github terhapus, oleh karena ini file dikirim ulang.
> _Keterangan file dikirim ulang karena yang sebelumnya foto tidakmuncul_
