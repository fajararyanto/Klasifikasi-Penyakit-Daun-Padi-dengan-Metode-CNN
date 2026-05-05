# Klasifikasi-Penyakit-Daun-Padi-dengan-Metode-CNN
Proyek ini adalah aplikasi web full-stack yang dirancang untuk deteksi otomatis penyakit pada daun padi. Pengguna dapat mengunggah gambar daun padi, dan sistem akan menganalisisnya menggunakan model machine learning yang telah dilatih sebelumnya. Aplikasi ini menyediakan informasi rinci tentang penyakit yang terdeteksi, termasuk deskripsi, metode pencegahan, dan rekomendasi kaya yang dihasilkan secara dinamis oleh Google Gemini API.

# Fitur

Frontend (Aplikasi React):

Autentikasi Pengguna: Registrasi dan login aman menggunakan JWT.
Unggah Gambar & Pindai Kamera: Pengguna dapat mengunggah gambar atau menggunakan kamera perangkat mereka (dengan kemampuan beralih kamera depan/belakang) untuk pemindaian real-time.
Deteksi Penyakit: Kirim gambar daun padi untuk analisis.
Hasil Analisis Rinci: Lihat prediksi penyakit, skor kepercayaan, deskripsi statis, metode pencegahan, dan wawasan yang dihasilkan AI dari Google Gemini.
Manajemen Profil Pengguna: Lihat dan edit detail profil pengguna.
Dasbor Admin: (Tersirat dari rute backend) Mengelola pengguna dan informasi penyakit.
Desain Responsif: Dioptimalkan untuk berbagai perangkat, termasuk seluler.
Backend (API Node.js & Express.js):

Manajemen Pengguna: Operasi CRUD untuk pengguna.
Autentikasi: Autentikasi berbasis JWT untuk akses API yang aman.
Manajemen Informasi Penyakit: Menyimpan dan mengambil data penyakit statis (deskripsi, pencegahan).
Penanganan Unggahan Gambar: Menggunakan multer untuk unggahan gambar yang efisien.
Integrasi Model Machine Learning: Mengintegrasikan model ResNet50v2 berformat ONNX untuk inferensi gambar menggunakan onnxruntime-node.
Integrasi Google Gemini API: Mengambil informasi dan rekomendasi dinamis yang kaya untuk penyakit yang terdeteksi.
Integrasi Basis Data: Menyimpan data pengguna, riwayat deteksi, dan informasi penyakit dalam basis data MySQL.
