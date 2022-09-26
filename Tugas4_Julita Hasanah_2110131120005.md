> Nama : Julita Hasanah<br>
> Nim : 2110131120005

<br><br>

<h1 align="center"><b>Struktur Sistem Operasi</b></h1>

<p align="justify">Sebuah sistem yang besar dan kompleks seperti sistem operasi modern harus diatur dengan cara membagi task kedalam komponen-komponen kecil agar dapat berfungsi dengan baik dan mudah dimodifikasi. Pada bab ini, kita akan membahas cara komponen-komponen ini dihubungkan satu sama lain. Menurut Silberschatz dan kawan-kawan, ada tiga cara yaitu:</p>

- Struktur Sederhana.
- Pendekatan Berlapis.
- Kernel Mikro.

<br>

## **Struktur Sederhana**

<p align="justify">Pada struktur ini, sistem operasi komputer dibuat dari sekumpulan prosedur, yang mana setiap prosedur itu dapat memanggil prosedur yang lainnya, kapan pun prosedur di perlukan. Pada struktur sederhana tidak ada pemisahan yang jelas antara aplikasi dan sistem operasi akibatnya program-program malware mudah memodifikasi dan merusak sistem operasi. Program aplikasi memiliki akses untuk memodifikasi bagian sistem operasi</p><br>

<p align="center"><img width="600px" src="gambarT4/1.jpg"><br></p>

Penjelasan lapisan gambar di atas

- Main Procedure adalah suatu program yang digunakan untuk memanggil salah satu dari service prosedures, dan juga meminta pelayanan dari service procedures.

- Service Prosedures adalah program yang diginakan untuk menjalankan fungsi pemanggilan procedures yang mana procedures itu harus di aktifkan.

- Utility Procedures adalah program dasar yang digunakan untuk mengendalikan sistem komputer dan juga untuk mengerjakan apa yang dibutuhkan oleh service procedures.

Contoh Sistem operasi yang menggunakan struktur ini adalah : UNIX , MS-DOS

<p align="center"><img width="800px" src="gambarT4/2.png"><br></p>

### **Keunggunlan**

- layanan dapat dilakukan sangat cepat karena terdapat di satu ruang alamat.

### **Kelemahan**

- Pengujian dan penghilangan kesalahan sulit karena tidak dapat dipisahkan dan dialokassikan.
- Sulit dalam menyediakan fasilitas pengamanan.
- Merupakan pemborosan bila setiap komputer harus mejalankan kerlel monolitik sangat besar smentara sbenarnya tidak memerlukan seluruh layanan yang disediakan kernel.
- Kesalahan pemrograman satu bagian dari kernel menyebabkan matinya seluruh sistem.

<br><br>

## **Sistem Berlapis (Layered)**

<p align="justify">Sistem operasi dibentuk secara hirarki berdasar lapisan — lapisan, dimana lapisan-lapisan bawa memberi layanan lapisan lebih atas. Lapisan yang paling bawah adalah bertugas menanngani ditil operasi perangkat keras dan yang paling tinggi menangani user- interface atau aplikasi.Rutin-rutin pada suatu lapisan hanya boleh menggunakan rutin-rutin lapisan bawahnya. Sebuah lapisan adalah implementasi dari obyek abstrak yang merupakan enkapsulasi dari data dan operasi yang bisa memanipulasi data tersebut. Struktur berlapis dimaksudkan untuk mengurangi kompleksitas rancangan dan implementasi sistem operasi. Contoh sistem operasi yang menggunakan sistem ini adalah: UNIX termodifikasi, THE, Venus dan OS/2.</p

**Sistem Berlapis Tanenbaum**<br>
<img width="450px" src="gambarT4/3.png"><br>
<br>
Menurut Tanenbaum dan Woodhull sistem berlapis terdiri dari enam lapisan, yaitu:

- **Lapisan 0**.Mengatur alokasi prosesor pertukaran antar proses ketika interupsi terjadi atau waktu habis.Lapisan ini mendukung dasar multi-programming pada CPU.

- **Lapisan 1**.Mengalokasikan ruang untuk proses di memori utama dan pada 512 kilo word drum yang digunakan untuk menahan bagian proses ketika tidak ada ruang dimemori utama.

- **Lapisan 2**.Menangani komunikasi antara masing-masing proses dan operator console.Pada lapisin imasing-masing proses secara efektif memiliki opertor console sendiri.

- **Lapisan 3**. Mengatur peranti M/K dan menampung informasi yang mengalir dari dan ke proses tersebut.

- **Lapisan 4**. Tempat program pengguna. Pengguna tidak perlu memikirkan tentang proses, memori, console, atau manajemen M/K.

- **Lapisan 5**. Merupakan operator sistem.

<br><br>

**Stallings memberi model yang lebih detail, sabagai berikut :**

- **Lapisan 1**. Berisi berbagai sirkuit elektronik, misalnya register , memory cells, dan logic gate.
- **Lapisan 2**. Berisi instruksi prosesor,misal instruksi aritmatika, instruksi transfer data,dsb.
- **Lapisan 3**. Penambahan konsep seperti prosedur/subrutin, maupun fungsi yang me-return nilai tertentu.
- **Lapisan 4**. Pemnambahan interrupt.
- **Lapisan 5**. Program sebagai sekumpulan instruksi yang dijalankan oleh prosesor.
- **Lapisan 6**. Berhubungan dengan secondary storage device, yaitu membaca/menulis head, track, dansektor.
- **Lapisan 7**. Menciptakan alamat logika untuk proses. Mengatur hubungan antara main memory,virtual memory,dan secondary memory.
- **Lapisan 8**. Program sebagai sekumpulan instruksi yang dijalankan oleh prosesor.
- **Lapisan 9**. Berhubungan dengan secondary storage device, yaitu membaca/menulis head, track, dansektor.
- **Lapisan 10**. Menciptakan alamat logika untuk proses. Mengatur hubungan antara main memory,virtual memory,dan secondary memory.
- **Lapisan 11**. Program sebagai sekumpulan instruksi yang dijalankan oleh prosesor.
- **Lapisan 12**. File adalah objek yang memiliki nama dan ukuran.Abstraksi dari lapisan 9.
- **Lapisan 13**. Menyediakan interface agar bisa berinteraksi dengan pengguna.

<br>

**Sistem Berlapis Stallings**<br>
<img width="450px" src="gambarT4/4.webp"><br>
<br>

Dapat disimpulkan bahwa lapisan sistem operasi secara umum terdiri atas empat bagian, yaitu :

1. **Perangkat keras**. Lebih berhubungan kepada perancang sistem. Lapisan ini mencakup lapisan 0 dan 1 menurut Tanenbaum, dan level 1 sampai dengan leve l3 menurut Stallings.
2. **Sistem operasi**. Lebih berhubungan kepada programer. Lapisan ini mencakup lapisan 2 menurut Tanenbaum, dan level 5 sampai dengan level 7 menurut Stallings.
3. **Kelengkapan**. Lebih berhubungan kepada programer. Lapisan ini mencakup lapisan 3 menurut Tanenbaum, dan level 8 sampai dengan level 11 menurut Stallings.
4. **Program aplikasi**. Lebih berhubungan kepada pengguna aplikasi komputer. Lapisan ini mencakup lapisan 4 dan lapisan 5 menurut Tanebaum, dan level 12 dan level 13 menurut Stallings.

<br>

### **Lapisan Sistem Operasi Secara Umum**<br>

<img width="450px" src="gambarT4/5.jpg"><br>
<br>

### **Keuntungan :**

- Mempermudah dubug dan verifikasi sistem
- Lapisan pertama bisa didebug tanpa menggangu sistem yang lain

<br>

### **Kesulitan :**

- hanya bisa menggunakan lapisan dibawahnya
- Tidak efisien dibandingkan tipe yang lain

<br><br>

## **Kernel Mikro**

<p align="justify">Mikrokernel adalah inti OS kecil yang menyediakan dasar untuk modular extensesi. Metode ini menyusun sistem operasi dengan menghapus semua komponen yang tidak esensial dari kernel, dan mengimplementasikannya sebagai program sistem dan level pengguna. Hasilnyakernelyang lebih kecil. Pada umumnya mikrokernel mendukung proses dan menagemen memori yang minimal, sebagai tambahan utnuk fasilitas komunikasi.<br><br>
Fungsi utama mikrokernel adalah mendukung fasilitas komunikasi antara program klien dan bermacam-macam layanan yang juga berjalan diuser space. Komunikasi yang dilakukan secara tidak langsung, didukung oleh sistem message passing, dengan bertukar pesan melalui mikrokernel.</p>
<br>

### **Keuntungan**

- **Interface** yang seragam. Proses tidak lagi dibedakan, baik antara kernel-level maupun user-level, karena semuanya berkomunikasi via message passing.
- **Extensibility**. Bisa menambahkan fitur-fitur baru tanpa perlu melakukan kompilasi ulang
- **Flexibility**. Fitur-fitur yang sudah ada bisa dikurangi, atau dimodifikasi sesuai dengan kebutuhan sehingga menjadi lebih efisien. Misalnya tidak semua pengguna membutuhkan security yang sangat ketat, atau kemampuan untuk melakukan distributed computing.
- **Portability**. Pada mikro kernel, semua atau sebagian besar kode yang prosesor-spesifik berada di dalamnya. Jadi, proses porting ke prosesor lain bisa dilakukan dengan relatif sedikit usaha. Pada kelompok desktop misalnya, tampaknya dominasi Intel makin kuat. Tapi, sampai seberapa lama itu bisa bertahan? Karena itulah, portability adalah salah satu isu yang sangat penting.
- **Reliability**. Semakin besar suatu software, maka tentulah semakin sulit untuk menjamin reliabilitynya. Desain dengan pendekatan berlapis sangatlah membantu, dan dengan pendekatan mikro kernel bisa lebih lagi. Mikro kernel dapat diuji secara ekstensif karena dia menggunakan API yang sedikit,sehingga bisa meningkatkan kualitas code di luar kernel.
- **Support for object-oriendted OS**. Model mikro kernel sangat sesuai untuk mengembangkan sistem operasi yang berbasis object-oriented. Contoh sistem operasi yang menggunakan mikro kernel adalah Mac OS X dan QNX.

<br>

### **Kinerjanya Mikrokernel**

<p align="justify">Dalam teorinya, sistem operasi yang menggunakan microkernel disebut jauh lebih stabil dibandingkan dengan monolithic kernel, karena sebuah server yang gagal bekerja, tidak akan menyebabkan kernel menjadi tidak dapat berjalan, dan server tersebut akan dihentikan oleh kernel utama. Akan tetapi, dalam prakteknya, bagian dari system state dapat hilang oleh server yang gagal bekerja tersebut, dan biasanya untuk melakukan proses eksekusi aplikasi pun menjadi sulit, atau bahkan untuk menjalankan server-server lainnya. Sistem operasi yang menggunakan microkernel umumnya secara dramatis memiliki kinerja di bawah kinerja sistem operasi yang menggunakan monolithic kernel. Hal ini disebabkan oleh adanya overhead yang terjadi akibat proses input/output dalam kernel yang ditujukan untuk mengganti konteks (context switch) untuk memindahkan data antara aplikasi dan server. Beberapa sistem operasi yang menggunakan microkernel:</p>

- IBM AIX, sebuah versi UNIX dari IBM
- Amoeba, sebuah kernel yang dikembangkan untuk tujuan edukasi
- Kernel Mach, yang digunakan di dalam sistem operasi GNU/Hurd, NexTSTEP, OPENSTEP, dan Mac OS/X
- Minix, kernel yang dikembangkan oleh Andrew Tanenbaum untuk tujuan
  edukasi
- Symbian OS, sebuah sistem operasi yang populer digunakan pada hand phone, handheld device, embedded device, dan PDA Phone.

<br>

<p align="center"><b>Struktur Sistem Operasi Berbasis Mikrokernel monolitik</b></p>
<p align="center"><img width="800px" src="gambarT4/6.png"><br></p>

<br>

### **Rancangan Mikrokernel**

<p align="justify">Pada pembahasan “Struktur Sederhana”, sempat disinggung istilah “kernel”. Kernel adalah komponen sentral dari sistem operasi. Ia mengatur hal-hal seperti interrupt handler(untuk menyediakan layanan interupsi), process scheduler(membagi-bagi proses dalam prosesor), memory management, I/O, dan sebagainya. Atau dengan kata lain, ia adalah jembatan antara hardware dengan software. Cara tradisional untuk membangun sistem operasi adalah dengan membuat kernel monolitis, yaitu semua fungsi disediakan oleh kernel, dan ini menjadikan kernel suatu program yang besar dan kompleks.<br><br>
Cara yang lebih modern, adalah dengan menggunakan kernel mikro. Pada awalnya, konsep mikro kernel dikembangkan pada sistem operasi Mach. Ide dasar dari pengembangan kernel mikro adalah bahwa hanya fitur-fitur yang perlu saja yang diimplementasikan dalam kernel (mengenai fitur-fitur apa saja yang perlu diimplementasikan, ini bisa berbeda tergantung desain sistem operasi).<br><br>
Walaupun garis pembatas mengenai apa saja yang berada di dalam dan luar kernel mikro bisa berbeda antara desain yang satu dengan yang lain, namun ada karakteristik yang umum, yaitu servis-servis yang umumnya menjadi bagian sistem operasi menjadi subsistem eksternal yang bisa berinteraksi satu sama lain dan dengan kernel tentunya. Ini mencakup device driver, file system, virtual memory manager, windowing system, dan security devices. Pendekatan kernel mikro menggantikan pendekatan berlapis yang vertikal tradisional.<br><br>
Komponen-komponen sistem operasi yang berada di luar kernel mikro diimplementasikan sebagai server process dan berkomunikasi dengan message passing via kernel mikro. Misalnya jika user ingin membuat berkas baru, dia mengirim pesan ke file system server, atau jika ingin membuat proses baru, dia mengirimkan pesan ke process server.</p>
