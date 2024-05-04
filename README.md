## Final Project Stage 2
- Berdasarkan data.info() tidak ditemukan data yang kosong atau hilang.
- Tidak terdapat kolom yang duplikat dari semua kolom
- Kita menghapus data outlier sekitar ~141 Baris dengan menggunakan z-score. Jumlah baris sebelum memfilter outlier: 10000 Jumlah baris setelah memfilter outlier: 9859
- Kita melakukan standarisasi untuk feature yang bertipe numeric agar skalanya cenderung sama.
- Kita melakukan feature Encoding terhadap 2 Feature:
Gender : label encoding
Geography: One Hot Encoding
- Karena data target kita tidak seimbang atau imbalance maka kami menggunakan oversampling SMOTE untuk membuat data seimbang.
Data awal : Original Exited (0=5485    1= 1416)
Data Setelah : Original Exited (0=5485    1= 5485)


- Feature Extraction
Balance_to_Salary_Ratio: Rasio antara saldo akun dan estimasi gaji pelanggan. Fitur ini mungkin dapat memberikan wawasan tentang bagaimana proporsi saldo akun pelanggan dibandingkan dengan besarnya estimasi gaji mereka.
Jika rasio ini tinggi, mungkin menunjukkan bahwa pelanggan memiliki saldo yang besar dibandingkan dengan pendapatannya, yang bisa menjadi indikasi kestabilan finansial atau potensi untuk menjadi nasabah yang berharga bagi bank.

Age_to_Tenure_Ratio: Rasio antara usia pelanggan dan masa jabatan (tenure) mereka di bank. Fitur ini dapat memberikan informasi tentang seberapa lama pelanggan telah menjadi nasabah bank relatif terhadap usia mereka.
Hal ini dapat membantu dalam memahami tingkat loyalitas pelanggan atau seberapa lama mereka telah terlibat dalam hubungan dengan bank.

