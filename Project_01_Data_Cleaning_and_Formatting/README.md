# Marvel Cinematic Universe Films and Series - Data Cleaning and Formatting

## 1. Latar Belakang

Proyek ini berawal dari rasa penasaran serta keinginan untuk mempraktikkan secara langsung materi _Data Cleaning_ yang telah dipelajari pada bab 3 modul kursus _Basic Excel for Data Analyst_. Guna menguji pemahaman pada studi kasus nyata, pencarian dataset mentah berformat `.CSV` dilakukan secara mandiri melalui platform Kaggle.com. Sebagai penggemar berat Marvel, saya memilih dataset Marvel Cinematic Universe untuk diproses dari kondisi mentah (_raw data_) hingga menjadi tabel yang rapi, konsisten, dan siap dianalisis.

## 2. Gambaran Umum Proyek

Proyek ini berfokus pada transformasi dataset Marvel Cinematic Universe (MCU) yang awalnya belum terstruktur, memiliki inkonsistensi format, dan sulit diolah, menjadi sebuah lembar kerja yang bersih, konsisten, dan sepenuhnya siap untuk tahap analisis data lebih lanjut (analytics-ready).

## 3. Sumber Data dan Referensi

- **Dataset Utama**: Marvel Cinematic Universe Films & Series (Berkas format .CSV bersumber dari Kaggle.com).
    
- Pengayaan dan Validasi Data:
    
    - **IMDb**: Validasi durasi film (*movie duration*) dan kelengkapan informasi dasar.
        
    - **Rotten Tomatoes**: Referensi skor *Tomato Meter* dan *Audience Score*.
        
    - **Box Office Mojo & The Numbers**: Validasi data finansial (anggaran produksi, pendapatan akhir pekan perdana, pendapatan domestik, serta total pendapatan global).
        

## Tools yang Digunakan

- **Microsoft Excel**
    

## Langkah Pembersihan Data

### 1. Pemisahan Data

Memisahkan data mentah berformat `.CSV` yang awalnya menumpuk dalam satu kolom tunggal agar terurai menjadi beberapa kolom terstruktur menggunakan fitur Text to Columns.

### 2. Penyesuaian Lebar Kolom dan Kerapihan Visual

Menerapkan fitur _Autofit Column Width_ serta penyesuaian manual untuk memastikan seluruh isi teks dan angka di setiap kolom dapat terbaca secara penuh tanpa terpotong.

### 3. Standardisasi Judul Film dan Konsistensi Teks

Menyesuaikan penulisan judul film dan serial agar presisi dan selaras dengan judul resminya. Menjaga kerapihan serta konsistensi kapitalisasi huruf dan tanda baca menggunakan _Find & Replace_.

### 4. Pemformatan Tipe Data dan Mata Uang

Mengubah angka mentah pada kolom finansial seperti _production_budget, opening_weekend, domestic_box_office, dan worldwide_box_office_ menjadi format mata uang dolar (`$`) secara konsisten. Menyeragamkan format tanggal pada kolom _release_date_ menjadi format `DD/MM/YYYY` serta merapikan penulisan durasi film.

### 5. Penanganan Data Berantakan dan Missing Values

Memperbaiki berbagai entri data yang dinilai berantakan atau tidak konsisten. Melengkapi data durasi film yang kosong secara mandiri berdasarkan pengalaman menonton, serta melengkapi sisanya melalui referensi eksternal yang valid (seperti IMDb, Rotten Tomatoes, Box Office Mojo, The Numbers, dan beberapa platform _streaming_). Menandai nilai finansial yang tidak dipublikasikan secara seragam menggunakan label `N/A`.

### 6. Penerapan Format Tabel dan Kustomisasi Estetika

Mengonversi rentang data biasa menjadi format tabel menggunakan pintasan `Ctrl + T`. Melakukan kustomisasi warna dan gaya tabel agar tampilan visual lebih estetis, profesional, dan memudahkan saat membaca per baris.

### 7. Pengaturan Tata Letak dan Cetak

Mengatur perataan teks (_alignment_) secara konsisten: teks rata kiri, angka/finansial rata kanan, serta tanggal rilis rata tengah. Melakukan pengaturan halaman (_Page Setup_) dalam orientasi lanskap dengan opsi _Fit to 1 Page Width_ serta menyelaraskan warna _header_ agar siap diekspor menjadi dokumen PDF maupun laporan visual.

## Before vs After

### Sebelum

![Raw_Data](/Project_01_Data_Cleaning_and_Formatting/Assets/before.png)

### Sesudah

![Cleaned_Data](/Project_01_Data_Cleaning_and_Formatting/Assets/After.png)