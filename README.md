# FutureMates

## **Deskripsi Proyek**
FutureMates adalah sebuah platform berbasis web yang dirancang untuk membantu individu, terutama siswa SMA dan lulusan baru, dalam menemukan jalur karier yang sesuai dengan minat dan kepribadian mereka. Menggunakan tes RIASEC sebagai dasar, FutureMates memberikan rekomendasi personal untuk pilihan karier, serta panduan mendalam tentang profesi yang cocok dengan hasil tes mereka.

---

## **Fitur Utama**
- **Tes RIASEC**: Platform ini menggunakan tes RIASEC untuk mengevaluasi minat dan kepribadian pengguna.
- **Rekomendasi Karier**: Memberikan daftar profesi atau jalur karier yang relevan berdasarkan hasil tes RIASEC.
- **Informasi Profesi**: Memberikan wawasan detail tentang profesi, seperti deskripsi pekerjaan, keterampilan yang dibutuhkan, dan prospek masa depan.
- **Aksesibilitas Web**: Dibangun dengan framework **Java Spring Boot** dan **Thymeleaf** untuk pengalaman pengguna yang optimal.

---

## **Teknologi yang Digunakan**
- **Backend**: Java Spring Boot (mengambil hasil dari API Python)
- **Frontend**: Thymeleaf Template Engine
- **Database**: MySQL
- **Keamanan**: Spring Security
- **Machine Learning**: Model klasifikasi berbasis RIASEC menggunakan Neural Networks

---

## **Dataset**
Proyek ini menggunakan dataset dari Kaggle:
[Holland Code RIASEC Test Responses](https://www.kaggle.com/datasets/lucasgreenwell/holland-code-riasec-test-responses)

Dataset ini berisi respons dari tes RIASEC yang digunakan untuk melatih model machine learning dalam memberikan rekomendasi yang akurat untuk jalur karier.

---

## **Cara Kerja Machine Learning**
Model pembelajaran mesin pada FutureMates:
1. **Input Data**: Mengambil respons tes RIASEC pengguna.
2. **Prediksi Jalur Karier**: Menggunakan Neural Networks untuk memprediksi minat karier berdasarkan respons tes.
3. **Rekomendasi**: Memberikan daftar profesi yang cocok dengan hasil prediksi.
4. **Detail Profesi**: Memberikan informasi tambahan mengenai pekerjaan, keterampilan yang dibutuhkan, dan prospek kerja.

---

## **Cara Instalasi dan Penggunaan**
1. Clone repositori ini:
   ```bash
   git clone https://github.com/AdrianID/FutureMates.git
   ```
2. Masuk ke direktori proyek:
   ```bash
   cd FutureMates/backend
   ```
3. Konfigurasi database di `application.properties`:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/futuremates
   spring.datasource.username=your_username
   spring.datasource.password=your_password
   ```
4. Jalankan aplikasi:
   ```bash
   ./mvnw spring-boot:run
   ```
5. Akses platform di browser:
   ```
   http://localhost:8080
   ```

---

## **Risiko dan Tantangan**
1. Dataset yang tidak lengkap dapat mempengaruhi akurasi model.
2. Tantangan teknis dalam deployment platform berbasis Java Spring Boot.
3. Potensi perbedaan performa pada perangkat pengguna.

---

## **Author**
- **Nama**: Adrian Frizna Affandi
- **Peran**: Pengembang Backend, Model Machine Learning, dan Antarmuka Web

---

## **Lisensi**
Proyek ini dilindungi oleh lisensi [MIT License](LICENSE).

---

## **Pengembangan Selanjutnya**
- Penambahan fitur simulasi pekerjaan berdasarkan profesi yang direkomendasikan.
- Integrasi dengan platform pencarian kerja atau portal lowongan.
- Peningkatan UI/UX untuk pengalaman pengguna yang lebih baik.

---

**FutureMates** \- Temukan karier impian Anda, mulai dari sini.
