# SaeStudioTools
generate A3 cutting, polaroid, potong
Berikut adalah file `README.md` yang disusun secara profesional untuk proyek **SAE Studio Tools** Anda:

# SAE Studio Tools – Digital Printing Workflow

**SAE Studio Tools** adalah kumpulan aplikasi berbasis web yang dirancang untuk mempercepat dan mempermudah alur kerja operasional di percetakan digital, khususnya untuk **SAE Xpress Bogor**. Alat ini memungkinkan operator cetak untuk melakukan pengaturan tata letak (*layouting*), pembuatan pola potong (*cutting patterns*), dan manajemen *bleed* secara otomatis tanpa perlu menggunakan software berat secara manual.

## 🚀 Fitur Utama

### 1. Alat Lebihan (Imposition & Bleed)
Fitur unggulan untuk menyusun gambar atau file PDF ke dalam area cetak kertas A3+ (32x48 cm).
* **Mirror Bleed Ganda**: Menambahkan lebihan secara otomatis sebesar 0.2 cm dengan logika pantulan cermin pada sisi kanan-kiri lalu atas-bawah agar sudut terisi sempurna.
* **Manual Crop**: Integrasi dengan `Cropper.js` untuk memotong area gambar secara presisi sesuai rasio ukuran target.
* **Dukungan Multi-Format**: Mendukung unggahan file gambar (JPG/PNG) dan PDF banyak halaman.
* **Smart Layout**: Fitur *Auto-Rotate* untuk mencari susunan paling efisien guna memaksimalkan jumlah gambar dalam satu lembar.
* **Perimeter Crop Marks**: Menghasilkan tanda potong vektor yang hanya berada di keliling terluar susunan gambar sesuai standar profesional.

### 2. Pola Cutting (Cutting Patterns)
Menyediakan berbagai pola jalur potong untuk mesin *plotter*.
* **Continuous Snaking Path**: Jalur potong ular (X dan Y) yang menyatu 100% untuk meminimalkan gerakan mata pisau naik-turun.
* **Diecut Contour**: Deteksi bentuk otomatis untuk gambar transparan dengan fitur *Auto-Bleed* 0.5 mm guna mencegah tepi putih setelah pemotongan.
* **Precision Circles**: Pembuatan pola lingkaran spiral dan lingkaran standar dengan diameter yang dapat disesuaikan (1 - 10 cm).

### 3. Polaroid Layout
Alat khusus untuk mengatur tata letak foto polaroid dengan berbagai pilihan ukuran, latar belakang, dan pemberian *watermark* otomatis.

## 🛠️ Teknologi yang Digunakan
* **HTML5 & CSS3**: Antarmuka modern dengan desain responsif menggunakan font *Plus Jakarta Sans* dan *DM Serif Display*.
* **JavaScript (Vanilla)**: Logika pemrosesan gambar dan kalkulasi grid.
* **jsPDF**: Perpustakaan utama untuk menghasilkan file PDF siap cetak dalam skala centimeter.
* **PDF.js**: Digunakan untuk merender file PDF kiriman pelanggan menjadi gambar resolusi tinggi (300 DPI).
* **Cropper.js**: Memberikan pengalaman potong gambar yang interaktif bagi pengguna.

## 📂 Struktur File
* `index.html`: Halaman utama (*landing page*) yang menampilkan navigasi ke semua alat.
* `lebihan.html`: Modul pengaturan *imposition* dan *bleed*.
* `cutting.html`: Modul pembuatan pola potong vektor.
* `polaroid.html`: Modul tata letak foto polaroid.
* `bigLogoSae.png`: Logo utama dengan efek *drop-shadow* hitam pekat.
* `favSae.png`: Ikon *favicon* untuk tab browser.

## 💻 Cara Penggunaan
1.  Buka file `index.html` pada peramban web (disarankan Google Chrome).
2.  Pilih alat yang ingin digunakan (contoh: Klik "Buka alat" pada kartu Lebihan).
3.  Unggah file yang akan diproses.
4.  Lakukan pengaturan orientasi, ukuran potong, dan jumlah salinan.
5.  Klik tombol **Download PDF** untuk mendapatkan file siap cetak.

---
**Versi 2.1.0** · Dikembangkan Ceel untuk operasional **SAE Xpress Bogor**.
