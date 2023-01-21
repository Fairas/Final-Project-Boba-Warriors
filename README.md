# Summary Insight

1. Dari visualisasi di atas dapat disimpulkan bahwa negara france dan Germany memiliki tingkat Churn yang sama dan negara Spain adalah negara dengan tingkat churn paling rendah, rekomendasi bisnis yang mungkin dapat di berikan adalah memrikan perlakuan khusu seperti customer engagement atau menawakan keuntungan jakngka panjang seperti membership program kepada France dan Germany
2. Dari visualisasi di atas dapat disimpulkan bahwa nasabah dengan masa tenure low lebih banyak atau kebanyakan nasabah bank mimiliki tenure kurang dari 4 tahun, rekomendasi bisnis yang mungkin di berikan adlah memberikan riward kepada nasabah dengan masa tenure tertentu agar supaya nasabah tetap bertahan dan tidak jdi churn.
3. Dari visualisasi di atas dapat disimpulkan bahwa nasabah yang memiliki credit score dibawah 400 akan cenderung melakukan churn, oleh karena itu kita dapat memperingati kepada perusahaan jika ada nasabah yang akan hit credit scorenya menjadi 400 kebawah, maka potensi churnnya akan lebih besar. Sehingga pihak bank dapat melakukan tindakan persuasi kepada nasabah tersebut seperti memberikan promo menarik.

# Data Pre-Processing

1. Setelah dilakukan pengecekan dengan .info() dan isna().sum() tidak di temukan mising value.
2. Setelah dilakukan pengecekan dengan duplicated().sum() tidak di temukan duplikat data.
3. Feature CreditScore, Age, Tenure, Balance, dan Estimated salary dari outlier difilter dengan menggunakan IQR yang hasilnya jumlah baris berkurang menjadi 9626.
4. Kolom Age dan Balance memiliki persebaran data right-skewed yang kemudian dilakukan transformasi data menggunakan standarisasi.
5. Encoding di lakukan pada kolom Geography dan Gender, pada kolom Geography dilakukan metode one hot encoding dan gender menggunakan metode label encoding.
6. Class imbalance telah dilakukan dan tiap kelas memiliki 7677 data.
7. Menghilangkan feature yang bersifat redundan yaitu Age_std dan Balance_std.
8. Menambahkan feature BalanceSalaryRatio.
9. Menambahkan feature AgeScore, CSunder400, CreditsSCore, dan TenureScore.
 