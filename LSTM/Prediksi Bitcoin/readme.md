## 🔥 Prediksi Harga Bitcoin dengan Machine Learning

![Bitcoin Prediction](https://upload.wikimedia.org/wikipedia/commons/4/46/Bitcoin.svg)

---

### 🚀 **Deskripsi Proyek**

Proyek ini merupakan implementasi **Machine Learning** untuk **memprediksi harga Bitcoin** menggunakan model **Long Short-Term Memory (LSTM)**. Model ini dilatih menggunakan data historis harga Bitcoin dan dievaluasi dengan berbagai metrik untuk memastikan keakuratannya.

### 📌 **Metodologi**

Pendekatan yang digunakan dalam proyek ini mengikuti tahapan berikut:

1️⃣ **Persiapan Data**

- Mengambil data historis harga Bitcoin.
- Mengubah format data agar sesuai untuk pemrosesan lebih lanjut.
- Memvisualisasikan data untuk memahami pola dan tren.
- Sumber data : 🔗 [📃Data Historis Bitcoin / USD](https://www.investing.com/crypto/bitcoin/btc-usd)

2️⃣ **Preprocessing Data**

- Melakukan **normalisasi** dengan **MinMaxScaler** untuk mempercepat konvergensi model.
- Membuat dataset dengan **look-back window** untuk menangkap pola waktu.

3️⃣ **Training Model**

- Membangun arsitektur **LSTM** yang optimal untuk data time series.
- Menggunakan **GridSearchCV** untuk menemukan kombinasi hyperparameter terbaik.
- Melatih model terbaik menggunakan **data latih**.

4️⃣ **Prediksi**

- Menggunakan model yang telah dilatih untuk memprediksi harga Bitcoin.
- Mengubah kembali hasil prediksi ke skala aslinya.

5️⃣ **Evaluasi**

- Mengevaluasi kinerja model dengan berbagai metrik akurasi.

6️⃣ **Visualisasi**

- Menampilkan hasil prediksi dan membandingkannya dengan data aktual.

---

### 🤖 **Algoritma yang Digunakan**

Model utama yang digunakan adalah **LSTM (Long Short-Term Memory)**, salah satu arsitektur **Recurrent Neural Network (RNN)** yang dirancang khusus untuk menangani data sekuensial seperti **time series**.

✅ **Kelebihan LSTM:**

- Dapat menangkap **pola jangka panjang** pada data historis.
- Mengatasi masalah **vanishing gradient** yang sering terjadi pada RNN biasa.
- Sangat cocok untuk **prediksi harga Bitcoin**, yang memiliki pola kompleks dan volatilitas tinggi.

---

### 📊 **Evaluasi Model**

Akurasi model dievaluasi menggunakan beberapa metrik berikut:

| **Metrik**                                | **Deskripsi**                                               |
| ----------------------------------------- | ----------------------------------------------------------- |
| **MSE (Mean Squared Error)**              | Rata-rata kuadrat selisih antara prediksi dan nilai aktual. |
| **RMSE (Root Mean Squared Error)**        | Akar dari MSE, lebih mudah diinterpretasikan.               |
| **MAE (Mean Absolute Error)**             | Rata-rata selisih absolut antara prediksi dan nilai aktual. |
| **MAPE (Mean Absolute Percentage Error)** | Kesalahan rata-rata dalam bentuk persentase.                |

Semakin rendah nilai dari metrik-metrik ini, semakin baik performa model.

---

### 🔍 **Penjelasan Detail**

📌 **1. Import Library**
Proyek ini menggunakan berbagai library populer seperti:

- `pandas` & `NumPy` untuk manipulasi data.
- `scikit-learn` untuk preprocessing & evaluasi.
- `TensorFlow` untuk membangun model LSTM.
- `Matplotlib` untuk visualisasi hasil.

📌 **2. Persiapan Data**

- Data harga Bitcoin diambil dari **sumber eksternal (CSV)**.
- Tipe data dikonversi agar kompatibel dengan model.
- Visualisasi data awal dilakukan untuk melihat pola tren.

📌 **3. Preprocessing Data**

- Data dinormalisasi menggunakan **MinMaxScaler** agar berada dalam rentang `[0,1]`.
- Dibuat **dataset dengan look-back window** (misalnya, menggunakan data 40 hari sebelumnya untuk memprediksi harga berikutnya).
- Data dibagi menjadi **training set dan test set**.

📌 **4. Pemodelan LSTM**

- Dibangun **model LSTM** dengan beberapa layer:
  - Layer LSTM untuk menangkap pola sekuensial.
  - Layer Dropout untuk menghindari overfitting.
  - Layer Dense untuk menghasilkan output prediksi.
- **Hyperparameter tuning** dilakukan dengan **GridSearchCV** untuk mendapatkan model terbaik.

📌 **5. Training & Prediksi**

- Model dilatih dengan **dataset training** hingga konvergen.
- Prediksi dilakukan terhadap **data test**.
- Hasil prediksi diubah kembali ke skala asli agar dapat dibandingkan dengan data aktual.

📌 **6. Evaluasi & Visualisasi**

- Hasil prediksi dievaluasi menggunakan **MSE, RMSE, MAE, dan MAPE**.
- Dibuat **grafik perbandingan** antara harga asli Bitcoin dan prediksi model.

---

### 📦 **Cara Menjalankan Proyek**

#### 1️⃣ **Clone Repository**

```bash
git clone https://github.com/username/repo-name.git
cd repo-name
```

#### 2️⃣ **Install Dependencies**

Pastikan kamu sudah menginstal **Python 3.x** dan jalankan:

```bash
pip install -r requirements.txt
```

#### 3️⃣ **Jalankan Script**

```bash
python train.py
```

#### 4️⃣ **Melihat Hasil Prediksi**

Hasil akan divisualisasikan dalam bentuk **grafik**.

---

### 🎯 **Kesimpulan**

✅ Model **LSTM** dapat digunakan untuk **memprediksi harga Bitcoin** dengan cukup akurat.  
✅ **Hyperparameter tuning** meningkatkan performa model.  
✅ Model perlu terus **diupdate dengan data terbaru** untuk mempertahankan akurasinya.

---

### 💡 **Pengembangan Selanjutnya**

🔹 Mencoba model **Transformer** untuk meningkatkan akurasi.  
🔹 Menggunakan **data fundamental Bitcoin** sebagai fitur tambahan.  
🔹 Membangun **API untuk real-time prediction**.

---

### 📌 **Kontributor**

👨‍💻 **Deo Rafiansyah Putra** – _Machine Learning Engineer_  
📧 Email: 210401179@student.umri.ac.id
🔗 GitHub: [Deo Rafiansyah dan Shelly 👻](https://github.com/deorafiansev)

---

⚡ **Jika proyek ini bermanfaat, jangan lupa ⭐ Star repo ini!** 😊
