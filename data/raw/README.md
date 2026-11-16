# Tugas 1: Akuisisi Data Nyata melalui Web Scraping atau API

* **Mata Kuliah:** Akuisisi dan Manajemen Data (BIFP-243)
* **Program Studi:** Informatika - Institut Bisnis dan Teknologi Indonesia (INSTIKI)
* **Nama Mahasiswa:** Ni PutuIndahning Sasmita
* **NIM:** 2501010104
* **Kelas:** F
* **Dosen Pengampu:** Dr. I Gede Totok Suryawan, S.Kom., M.T.

---

## 1. Sumber Data
* **Nama Sumber:** OpenStreetMap (Overpass API) - Data Pariwisata & Kuliner Wilayah Denpasar
* **URL:** https://overpass-api.de/api/interpreter
* **Penerbit:** OpenStreetMap Contributors

## 2. Tanggal dan Jam Akses
* **Tanggal:** 16 November 2026
* **Jam:** 20:30 WITA

## 3. Metode Akuisisi (API)
* **Teknik:** Mengambil data melalui Overpass API (OpenStreetMap) tanpa API key menggunakan metode HTTP POST di Python.
* **Parameter & Konfigurasi:** Menggunakan query Overpass QL untuk memfilter fasilitas pariwisata (`tourism`) dan restoran/kafe (`amenity`) di sekitar wilayah koordinat Denpasar dengan limit 150 record.

## 4. Batasan Etika
* Mematuhi lisensi ODbL dengan mencantumkan atribusi sumber "© OpenStreetMap contributors".
* Menggunakan parameter *timeout* dan tidak melakukan *spam* atau *query* berulang yang membebani server publik.
* Hanya mengambil data fasilitas umum/publik tanpa melibatkan data privat atau sensitif individu.

## 5. Penjelasan Singkat Kolom Dataset (`data/raw/osm_denpasar_20261116.csv`)
1. `id_osm`: Identifikasi unik objek data dari OpenStreetMap.
2. `nama_tempat`: warung mak beng sanur
3. `kategori`: Klasifikasi jenis tempat restoran
4. `wilayah`: Denpasar
5. `latitude`: Titik koordinat garis lintang (latitude).
6. `longitude`: Titik koordinat garis bujur (longitude).

## 6. Cara Menjalankan Ulang Notebook
1. Pastikan pustaka Python yang dibutuhkan terinstal:
   ```bash
   pip install requests pandas
