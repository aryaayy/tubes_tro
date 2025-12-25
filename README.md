# OPTIMASI JARINGAN TRANSSHIPMENT SAMPAH DUA TINGKAT (TWO-ECHELON) MENGGUNAKAN ALGORITMA SPLIT DELIVERY VRP BERBASIS OPENSTREETMAP DI KOTA BANDUNG

## Struktur Folder Project
* **dataset**: Berisi data-data mentah yang digunakan untuk menjalankan algoritma transshipment.
    * **fasilitas_full.csv**: Data TPS yang ada di Kota Bandung.
    * **Jumlah Penduduk Kota Bandung menurut Kecamatan, 2024.csv**: Data jumlah penduduk Kota Bandung per Kecamatan pada tahun 2024.
    * **jumlah_capaian_penanganan_sampah_di_kota_bandung.csv**: Data capaian penanganan sampah di Kota Bandung per bulan dari tahun 2017 - 2024.
    * **jumlah_produksi_sampah_menurut_jenisnya_di_kota_ban_1.csv**: Data produksi sampah berdasarkan jenisnya di Kota Bandung dari tahun 2018 - 2024.
    * **jumlah_ritasi_pengangkutan_sampah_di_kota_bandung_1.csv**: Data ritase pengangkutan sampah di Kota Bandung per bulan dari tahun 2017 - 2024.
    * **final_dataset_2echelon.csv**: Data hasil praproses yang berisi join antara data kecamatan dan data fasilitas TPS, serta asumsi cost pengangkutan sampah dari rumah warga ke tps.
    * **distance_matrix_osrm.json**: Data distance matrix yang berisi jarak dari tiap fasilitas ke fasilitas lain.
    * **tabel_analisis_operasional.csv**: Summary data hasil modelling yang dikelompokkan berdasarkan jumlah ritase.
* **notebook**: Berisi kode program utama untuk menjalankan algoritma transshipment dan visualisasi.
    * **preprocessing.ipynb**: Praproses dataset awal agar siap digunakan untuk modelling.
    * **modelling.ipynb**: Script berisi algoritma transshipment menggunakan data hasil praproses.
    * **visualisasi_tps.ipynb**: Memvisualisasikan sebaran TPS, Pool Armada, dan TPA di kota bandung.
    * **visualisasi_rute.ipynb**: Memvisualisasikan hasil modelling berupa rute jalan optimal pada peta.
    * **visualisasi_laporan.ipynb**: Memvisualisasikan laporan data hasil modelling menjadi beberapa grafik.
* **results**: Berisi data-data hasil modelling.
    * **optimized_routes.json**: Data hasil modelling berupa detail perjalanan tiap kendaraan.
    * **reports.txt**: Data summary hasil modelling.
* **figures**: Berisi hasil visualisasi.