## Cara Kerja Metode IQR untuk Menghilangkan Outlier
**IQR (Interquartile Range)** adalah selisih antara kuartil ke-3 (Q3) dan kuartil ke-1 (Q1) dari data.
**Langkah utama:**
- Hitung Q1 (nilai pada persentil ke-25).
- Hitung Q3 (nilai pada persentil ke-75).
- Hitung IQR = Q3 - Q1.
- Tentukan batas bawah dan batas atas: Batas bawah = Q1 - 1.5 * IQR. Batas atas = Q3 + 1.5 * IQR
- Data yang berada di luar batas bawah dan batas atas dianggap outlier.
- Buang data outlier tersebut dari dataset.

**Mengapa metode ini efektif?**
- Tidak terpengaruh nilai ekstrem seperti rata-rata.
- Cocok untuk data yang tidak berdistribusi normal.
- Menghilangkan data "ngawur" atau ekstrem yang bisa mengganggu analisis.
