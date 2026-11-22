# ChronoTherapy AI — Premium v6 Research Workspace

Prototipe aplikasi penelitian prediksi kronoterapi untuk penentuan waktu pemberian obat antihipertensi.

**Pengembang:** apt. Fendy Prasetyawan, S.Farm., M.Farm.

**Judul disertasi:** Pengembangan Model Prediksi Kronoterapi Berbasis Machine Learning untuk Penentuan Waktu Pemberian Obat Antihipertensi.

## Empat modul yang ditambahkan
1. **ABPM Analysis:** input pembacaan berwaktu dengan kategori terjaga/tidur; hitung rerata SBP/DBP dan persentase penurunan malam dari rerata periode. Minimal dua pembacaan valid per periode diperlukan hanya untuk pratinjau hitung aplikasi; hal ini bukan kriteria kecukupan ABPM klinis.
2. **Drug Profile:** catat obat, golongan, formulasi, durasi kerja yang tercantum, frekuensi, dan waktu pemberian saat ini. Sebagian informasi ini hanya dicatat sebagai konteks, belum menjadi fitur prediktor model.
3. **Model Interpretation:** menampilkan kepentingan fitur global dari pemisahan pohon pada model prototipe. Ini bukan penjelasan kausal atau bukti klinis individual.
4. **Clinical Research Report:** menyusun laporan dan membuka dialog cetak browser; pilih “Save as PDF” untuk menyimpan sebagai PDF.

## Status dan batasan model
Model Random Forest pada prototipe masih bersifat eksperimental, menggunakan label demonstrasi yang dibangkitkan secara programatis, bukan luaran pasien. Model belum diuji pada data pasien nyata, belum menjalani validasi eksternal, dan tidak boleh digunakan untuk menetapkan atau mengubah terapi. Penggunaan klinis membutuhkan data sah secara etik, definisi luaran yang dapat dipertanggungjawabkan, pelatihan/pengujian terpisah, kalibrasi, validasi eksternal, serta pengawasan klinis.

## Privasi
Versi ini memproses masukan di browser; tidak ada backend atau database. Hindari memasukkan nama, nomor rekam medis, alamat, atau data yang dapat mengidentifikasi pasien. Gunakan kode subjek penelitian.

## Instalasi melalui GitHub Pages
1. Ekstrak ZIP dan unggah seluruh isi folder proyek ke root repository, dengan `index.html` di root.
2. Buka **Settings → Pages → Deploy from a branch**.
3. Pilih branch `main` dan folder `/ (root)`, lalu **Save**.
4. Buka alamat GitHub Pages. HTTPS diperlukan untuk service worker/PWA.
5. Untuk menyimpan PDF, gunakan tombol **Cetak / Simpan PDF**, kemudian pilih **Save as PDF** pada dialog cetak browser.
