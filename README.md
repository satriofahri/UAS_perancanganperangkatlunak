# UAS_perancanganperangkatlunak
Sistem Informasi Pendaftaran dan Pengelolaan Data Mahasiswa UKM Badminton Berbasis Web

1.	Permasalahan
Unit Kegiatan Mahasiswa (UKM) Badminton di Universitas Tangerang Raya merupakan salah satu wadah untuk mengembangkan minat, bakat, dan prestasi mahasiswa dalam bidang olahraga. Namun, pengelolaan administrasi dan data peserta UKM ini masih dilakukan secara manual atau menggunakan cara-cara yang kurang terstruktur. Hal ini mengakibatkan berbagai permasalahan, di antaranya:
A.	Proses Pendaftaran yang Tidak Praktis:
Calon peserta harus mendaftar dengan mengisi formulir secara manual atau melalui aplikasi sederhana yang tidak terintegrasi, sehingga memakan waktu lebih lama dan berpotensi menyebabkan kehilangan data.
B.	Data Peserta Tidak Tersentralisasi:
Informasi tentang peserta, seperti biodata, jadwal latihan, dan statistik kehadiran, tersebar di berbagai dokumen atau file, sehingga sulit untuk dikelola dan diperbarui secara efisien.
C.	Rentan Terhadap Kesalahan Data:
Penginputan data secara manual sering kali menimbulkan kesalahan, baik dalam pencatatan identitas peserta, kehadiran, maupun jadwal kegiatan, yang dapat menghambat operasional UKM.
D.	Keterbatasan Pemantauan dan Pelaporan:
Pengurus UKM kesulitan memantau perkembangan peserta, seperti kehadiran dan capaian latihan, karena tidak adanya sistem pelaporan yang terstruktur dan mudah diakses.
E.	Minimnya Akses Informasi bagi Peserta dan Pengurus:
Informasi penting seperti jadwal latihan, pengumuman, dan laporan kehadiran tidak dapat diakses secara real-time oleh peserta atau pengurus, sehingga mengurangi transparansi dan efektivitas koordinasi.

2.	Saran Solusi
Untuk memenuhi kebutuhan sistem informasi berbasis web yang fokus pada pendaftaran dan penyimpanan data mahasiswa untuk UKM Badminton di Universitas Tangerang Raya, solusi yang diusulkan adalah:
A.	Penggunaan Teknologi:
o	Bahasa Pemrograman: PHP untuk logika aplikasi.
o	Database: MySQL untuk penyimpanan data mahasiswa secara terpusat.
o	Frontend: Framework Bootstrap untuk membuat antarmuka yang responsif dan mudah digunakan.
o	Web Server: Menggunakan XAMPP untuk pengembangan lokal atau server berbasis LAMP untuk implementasi live.
B.	Fitur Utama Sistem dengan Metode CRUD:
o	Formulir Pendaftaran Mahasiswa (Create):
	Mahasiswa dapat mengisi formulir pendaftaran online yang mencakup data seperti nama, NIM, jurusan, nomor kontak, dan alamat email.
	Data yang diinput akan divalidasi sebelum disimpan ke dalam database MySQL.
o	Daftar Data Mahasiswa (Read):
	Admin dapat melihat daftar mahasiswa yang telah mendaftar dalam bentuk tabel.
	Tabel dilengkapi dengan fitur pencarian, filter, dan paginasi untuk memudahkan pengelolaan data.
o	Pembaruan Data Mahasiswa (Update):
	Admin dapat memperbarui informasi mahasiswa, misalnya jika ada kesalahan penulisan nama atau kontak yang berubah.
	Halaman edit data akan menampilkan formulir dengan data mahasiswa yang telah terisi sebelumnya.
o	Penghapusan Data Mahasiswa (Delete):
	Admin dapat menghapus data mahasiswa yang tidak valid atau tidak aktif melalui tombol hapus pada daftar mahasiswa.
C.	Keamanan Sistem:
o	Sistem dilengkapi dengan autentikasi pengguna berbasis login untuk admin, sehingga hanya pihak yang berwenang yang dapat mengakses data mahasiswa.
o	Validasi input di sisi server untuk mencegah serangan seperti SQL Injection.
o	Kata sandi admin akan disimpan dalam database menggunakan enkripsi seperti bcrypt.
D.	Desain Sederhana dan Efisien:
o	Antarmuka dibuat sederhana dengan fokus pada kemudahan pendaftaran dan pengelolaan data.
o	Hanya fungsi-fungsi utama (pendaftaran, lihat data, edit, dan hapus) yang diimplementasikan untuk menjaga sistem tetap ringan dan mudah digunakan.
E.	Output Data:
o	Data mahasiswa dapat diekspor dalam format Excel jika diperlukan untuk keperluan dokumentasi atau laporan.


3.	Perancangan
Skema Hardware
Untuk membangun dan menjalankan Sistem Informasi Pendaftaran dan Pengelolaan Data Mahasiswa UKM Badminton Berbasis Web di Universitas Tangerang Raya, berikut adalah perangkat keras yang dibutuhkan:
A.	Server (Hosting)
•	Fungsi: Menyimpan dan menjalankan aplikasi web serta database.
•	Deskripsi: Server akan digunakan untuk men-deploy sistem informasi secara online sehingga dapat diakses oleh mahasiswa untuk mendaftar dan oleh pengurus UKM untuk mengelola data.
•	Spesifikasi:
o	Processor: Intel Xeon E3 atau setara
o	RAM: 8 GB (minimal)
o	Storage: 100 GB SSD (untuk menyimpan data aplikasi, database, dan file lainnya)
o	OS: Linux (Ubuntu/Debian) atau Windows Server
o	Koneksi Internet: Kecepatan tinggi dan stabil untuk memastikan akses aplikasi berjalan lancar tanpa gangguan
B.	 Workstation (PC atau Laptop untuk Admin)
•	Fungsi: Digunakan oleh pengurus atau admin untuk mengelola data peserta, memproses pendaftaran, memperbarui informasi mahasiswa, dan menghasilkan laporan.
•	Deskripsi: Admin akan mengakses aplikasi berbasis web melalui browser di perangkat workstation untuk melakukan tugas administratif.
•	Spesifikasi:
o	Processor: Intel i3 (atau setara) atau lebih tinggi
o	RAM: 4 GB atau lebih
o	Storage: 500 GB HDD atau 256 GB SSD
o	Monitor: Ukuran layar minimal 15 inci
o	OS: Windows 10 atau macOS, atau sistem operasi berbasis Linux
C.	 Perangkat Pengguna (Mahasiswa)
•	Fungsi: Mahasiswa menggunakan perangkat ini untuk mendaftar dan mengakses informasi terkait pendaftaran dan data mereka.
•	Deskripsi: Mahasiswa akan mengakses sistem menggunakan perangkat pribadi, seperti komputer desktop, laptop, atau ponsel pintar, yang terhubung ke internet.
•	Spesifikasi:
o	Laptop/PC atau Smartphone: Laptop dengan spesifikasi yang sama dengan workstation, atau smartphone dengan sistem operasi Android/iOS.
o	Koneksi Internet: Diperlukan akses internet untuk pendaftaran online dan penggunaan aplikasi berbasis web.
D.	 Router dan Jaringan Lokal (LAN/WiFi)
•	Fungsi: Menyediakan konektivitas jaringan yang stabil antara server dan perangkat pengakses sistem.
•	Deskripsi: Router yang mendukung koneksi internet dengan bandwidth tinggi untuk memastikan kinerja aplikasi web yang lancar dan koneksi jaringan yang stabil untuk mahasiswa dan pengurus yang mengakses aplikasi di kampus.
•	Spesifikasi:
o	Router: Router dengan kecepatan internet minimal 100 Mbps
o	WiFi: Akses WiFi dengan sinyal kuat dan jangkauan yang luas di area kampus
E.	 Backup Storage (Opsional)
•	Fungsi: Sebagai cadangan untuk data penting dan pengelolaan file yang aman.
•	Deskripsi: Backup storage akan digunakan untuk memastikan bahwa data peserta dan aplikasi dapat dipulihkan jika terjadi masalah atau kehilangan data pada server utama.
•	Spesifikasi:
o	Storage: 500 GB HDD atau 256 GB SSD (dapat menggunakan layanan cloud storage seperti Google Drive atau Dropbox sebagai alternatif)

Skema Software:
Untuk mengembangkan Sistem Informasi Pendaftaran dan Pengelolaan Data Mahasiswa UKM Badminton Berbasis Web, berikut adalah arsitektur software dan alat bantu yang digunakan:
1. Arsitektur Software
Sistem menggunakan arsitektur berbasis Client-Server dengan model 3-Tier Architecture, yang terdiri dari tiga lapisan utama:
a. Presentation Layer (Frontend)
•	Fungsi: Menyediakan antarmuka pengguna untuk mahasiswa dan admin agar dapat berinteraksi dengan sistem.
•	Komponen:
o	HTML, CSS: Digunakan untuk membangun struktur dan tampilan halaman web.
o	Framework Bootstrap: Untuk desain responsif dan komponen UI.
•	Tools: Text editor seperti Visual Studio Code.
b. Application Layer (Backend)
•	Fungsi: Menangani logika aplikasi dan mengelola komunikasi antara frontend dan database.
•	Komponen:
o	PHP: Untuk menangani logika CRUD dan memproses data.
o	XAMPP: Untuk menjalankan server lokal berbasis Apache dan PHP.
•	Framework: Penggunaan PHP Native atau framework seperti CodeIgniter jika diperlukan.
c. Data Layer (Database)
•	Fungsi: Menyimpan data peserta dan menyediakan akses data yang efisien untuk backend.
•	Komponen:
o	MySQL: Sistem manajemen database relasional untuk menyimpan data peserta secara terstruktur.
•	Tools: phpMyAdmin untuk pengelolaan database.
2. Alat Bantu (Tools) yang Digunakan
a. Pengembangan
•	Text Editor:
o	Visual Studio Code sebagai editor kode untuk pengembangan frontend dan backend.
•	Server Lokal:
o	XAMPP untuk menjalankan server lokal (Apache) dan database (MySQL).
b. Desain dan Dokumentasi
•	Lucidchart atau Draw.io: Untuk menggambarkan diagram seperti ERD (Entity-Relationship Diagram) dan Flowchart.
c. Pengujian
•	Browser Developer Tools: Untuk debug frontend (HTML, CSS, php).
d. Manajemen Proyek
•	Google Docs/Sheets: Untuk dokumentasi dan kolaborasi tim.


Skema database (class diagram)

Skema actor
1.	Use case diagram

2.	Sequence diagram

3.	Activity diagram

Coding
•	Bahasa Pemrograman:
Sistem ini dibangun menggunakan bahasa PHP untuk logika backend dan SQL untuk manajemen database.
•	Framework atau Tools: 
o	Bootstrap: Digunakan untuk merancang antarmuka pengguna (UI) yang responsif.
o	phpMyAdmin: Untuk mengelola database MySQL.
o	XAMPP: Sebagai server lokal untuk menjalankan aplikasi berbasis web.
•	Berbasis:
Aplikasi ini berbasis web, sehingga dapat diakses melalui browser oleh pengguna.
Gambar codingan sebagai berikut:
 
Implementasi
1.	Setup Server Lokal:
o	Instalasi XAMPP pada komputer lokal.
o	Konfigurasi Apache dan MySQL untuk menjalankan aplikasi.
2.	Desain Database:
o	Membuat tabel untuk admin dan mahasiswa di phpMyAdmin.
o	Menetapkan relasi antara tabel admin dan mahasiswa melalui Foreign Key (admin_id).
3.	Pengembangan Fitur CRUD:
o	Create: Formulir untuk menambahkan data mahasiswa.
o	Read: Menampilkan daftar mahasiswa yang terdaftar.
o	Update: Mengedit data mahasiswa yang sudah ada.
o	Delete: Menghapus data mahasiswa tertentu.
4.	Implementasi UI/UX:
o	Menggunakan Bootstrap untuk membuat halaman web yang responsif dan user-friendly.
o	Desain halaman meliputi: Login admin, dashboard, dan formulir pendaftaran mahasiswa.
5.	Pengujian Awal:
o	Menjalankan aplikasi di localhost untuk memastikan tidak ada error dalam fungsi dasar sistem.
6.	Deployment (Opsional):
Jika diperlukan, aplikasi dapat diunggah ke hosting untuk digunakan secara online.
Berikut gambar tampilan databasenya
 
Testing
1.	Unit Testing:
o	Menguji fungsi individual seperti proses pendaftaran mahasiswa, pengeditan data, dan penghapusan.
o	Tools yang digunakan: Debugging PHP secara manual melalui browser dan log error.
2.	Integration Testing:
o	Menguji hubungan antar modul, seperti integrasi antara formulir pendaftaran dengan database.
o	Memastikan alur CRUD berjalan tanpa konflik.
3.	User Acceptance Testing (UAT):
o	Mengundang pengguna akhir (admin dan mahasiswa) untuk mencoba aplikasi.
o	Memastikan bahwa sistem sesuai dengan kebutuhan dan mudah digunakan.
4.	Performance Testing:
o	Mengukur waktu respon aplikasi untuk memastikan tidak ada keterlambatan signifikan dalam proses CRUD.
o	Menggunakan XAMPP untuk memonitor penggunaan resource sistem selama pengujian.
Berikut adalah tampilan websitenya
 
