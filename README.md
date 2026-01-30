📊 Segmentasi Nasabah Berpotensi Tinggi untuk Investasi Jangka Panjang (Deposito)

- Author: Aqila Khansa Hartanto
- Project Type: Exploratory Data Analysis & Customer Segmentation
- Domain: Banking / Customer Analytics / Customer Lifetime Value (CLV)

📌 Project Overview

Bank ingin meningkatkan Customer Lifetime Value (CLV) dengan mendorong nasabah existing untuk berinvestasi pada produk simpanan jangka panjang (deposito). Namun, tidak semua nasabah memiliki ketertarikan dan kapasitas finansial yang sama.

Project ini bertujuan untuk:
1. Menganalisis hubungan profil nasabah dengan keputusan berlangganan deposito
2. Mengidentifikasi pola usia, saldo, dan status pinjaman
3. Menentukan tipe nasabah paling potensial untuk ditargetkan oleh Relationship Manager
4. Pendekatan yang digunakan bersifat EDA-driven dan rule-based segmentation, sehingga hasilnya mudah dipahami dan langsung aplikatif secara bisnis.

🧩 Dataset

Dataset berisi informasi profil nasabah bank, antara lain:
- Demografi (usia, pekerjaan, pendidikan, status pernikahan)
- Informasi finansial (saldo rata-rata, kepemilikan pinjaman, kartu kredit)
- Interaksi bank (channel kontak, relationship manager contact)
- Target: subscription deposito (Yes/No)

🛠 Tools & Libraries

1. Python
2. Pandas & NumPy – data processing
3. Matplotlib – data visualization
4. YData Profiling – exploratory data profiling
5. Google Colab – development environment

🔍 Analysis Workflow
1️⃣ Exploratory Data Analysis (EDA)
- Profiling data untuk mengecek struktur, tipe data, dan kualitas data
- Analisis distribusi target (subscription deposito)

2️⃣ Preprocessing
- Menghapus kolom tidak relevan (customer_id)
- Standarisasi nama kolom
- Encoding target (subscription)
- Pengelompokan usia dan saldo
- Penanganan data kategorikal untuk analisis EDA

3️⃣ Task 1 – Profil Nasabah vs Keputusan Deposito

Analisis hubungan antara:
1. Pekerjaan
2. Pendidikan
3. Status pernikahan
4. Channel kontak
5. Status pinjaman
6. Pengalaman investasi
7. Interaksi dengan relationship manager

Insight utama:
Nasabah dengan profil finansial yang stabil, pengalaman investasi, serta interaksi langsung dengan RM menunjukkan tingkat berlangganan deposito yang jauh lebih tinggi.

4️⃣ Task 2 – Pola Usia, Saldo, dan Status Pinjaman
- Usia dikelompokkan (<30, 30–40, 40–50, 50–60, >60)
- Saldo dikelompokkan menggunakan quartile (q=4)
- Analisis personal loan & housing loan

Insight utama:
Nasabah usia >40 tahun dengan saldo tinggi dan tanpa beban cicilan perumahan memiliki kecenderungan paling kuat untuk berlangganan deposito.

5️⃣ Task 3 – Segmentasi Nasabah Potensial
Segmentasi rule-based untuk mengidentifikasi High Potential Customers berdasarkan:
1. Sudah berlangganan deposito
2. Saldo tinggi / sangat tinggi
3. Usia ≥ 40 tahun
4. Tidak memiliki personal loan

📌 Ringkasan Segmentasi
| Segmen             | Rata-rata Usia | Rata-rata Saldo | Proporsi Deposito |
| ------------------ | -------------- | --------------- | ----------------- |
| High Potential     | ± 51 tahun     | ± 25 juta       | 100%              |
| Non High Potential | ± 34 tahun     | ± 5 juta        | 6%                |


💡 Key Business Insight

Nasabah dengan usia matang dan saldo tinggi merupakan segmen kecil namun memiliki tingkat konversi deposito yang sangat tinggi. Segmen ini ideal untuk pendekatan personal oleh Relationship Manager guna memaksimalkan CLV dibandingkan kampanye massal.


