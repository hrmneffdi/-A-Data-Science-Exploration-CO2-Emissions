# Eksplorasi Emisi CO2 : Pendekatan Data Science untuk Analisis Dampak Lingkungan
![Gambar Ilustrasi](https://github.com/hrmneffdi/-A-Data-Science-Exploration-CO2-Emissions/blob/main/image_fixx.jpeg)
## Pendahuluan

Perubahan iklim akibat akumulasi emisi CO2 memiliki dampak lingkungan yang signifikan, termasuk pemanasan global, kenaikan permukaan laut, perubahan pola cuaca, dan gangguan ekosistem. Proyek analisis emisi CO2 ini menggunakan pendekatan Data Science untuk mengidentifikasi tren, pola, serta solusi potensial dalam mengurangi emisi CO2. Analisis dilakukan pada dataset yang mencakup variabel kendaraan dan faktor terkait untuk memberikan wawasan mendalam mengenai kontribusi emisi CO2 dari sektor kendaraan dan merumuskan rekomendasi penting untuk pengurangan dampak lingkungan yang merugikan.

## Tujuan

Tujuan utama proyek ini adalah menganalisis data emisi CO2 menggunakan pendekatan Data Science untuk mengidentifikasi pola, tren, dan hubungan antara variabel kendaraan dan emisi CO2. Proyek juga bertujuan mengembangkan model prediksi emisi CO2 untuk memberikan wawasan tentang kontribusi faktor terhadap emisi dan solusi potensial mengurangi dampak lingkungan akibat emisi CO2.

## Pertanyaan Penelitian

1. Apakah ukuran mesin kendaraan mempengaruhi tingkat emisi CO2?
2. Bagaimana hubungan antara jumlah silinder mesin dan emisi CO2?
3. Apakah jenis transmisi kendaraan berdampak pada tingkat emisi CO2?
4. Bagaimana perbandingan emisi CO2 antara kendaraan yang menggunakan bahan bakar berbeda?
5. Apakah terdapat korelasi antara efisiensi bahan bakar dan emisi CO2?
6. Bagaimana hubungan antara konsumsi bahan bakar miles per gallon (mpg) terhadap emisi CO2?

## Workflow Proyek

- **Pengumpulan Data**: Penjelasan tentang bagaimana data dikumpulkan.

- **Analisis Data Eksploratori**: Gambaran tentang karakteristik, pola, dan hubungan variabel untuk menjawab pertanyaan penelitian.

- **Pra-pemrosesan Data**: Penjelasan tentang persiapan data sebelum pembangunan model Machine Learning.

- **Pembangunan dan Evaluasi Model**: Penjelasan algoritma Machine Learning yang digunakan dan evaluasi model prediksi.

- **Kesimpulan**: Rekomendasi dari hasil analisis untuk mengurangi emisi CO2.

## Pengumpulan Data

Dataset relevan untuk analisis emisi CO2 diperoleh dari Kaggle, yang memberikan akses ke data terstruktur. Langkah-langkah pengumpulan data melibatkan:

- **Identifikasi Sumber Data**: Memilih dataset CO2 Emissions.csv yang menyediakan karakteristik kendaraan dan emisi CO2.

- **Pemahaman Terhadap Data**: Memahami variabel-variabel yang ada dalam dataset:

  a. **Make**: Merek (pembuat) kendaraan.<br>
   b. **Model**: Model kendaraan.<br>
   c. **Vehicle Class**: Kelas kendaraan.<br>
   d. **Engine Size (L)**: Ukuran mesin kendaraan dalam liter.<br>
   e. **Cylinders**: Jumlah silinder dalam mesin kendaraan.<br>
   f. **Transmission**: Jenis transmisi kendaraan.<br>
   g. **Fuel Type**: Jenis bahan bakar yang digunakan.<br>
   h. **Fuel Consumption City (L/100 km)**: Konsumsi bahan bakar dalam kota dalam liter per 100 km.<br>
   i. **Fuel Consumption Hwy (L/100 km)**: Konsumsi bahan bakar di jalan raya dalam liter per 100 km.<br>
   j. **Fuel Consumption Comb (L/100 km)**: Konsumsi bahan bakar gabungan dalam liter per 100 km.<br>
   k. **Fuel Consumption Comb (mpg)**: Konsumsi bahan bakar gabungan dalam mil per galon.<br>
   l. **CO2 Emissions (g/km)**: Emisi CO2 dalam gram per kilometer.<br>


## Analisis Data Eksploratori

Pada tahap ini, kami melakukan Exploratory Data Analysis (EDA) untuk memberikan ringkasan tentang karakteristik, pola, serta hubungan antar variabel dalam rangka menjawab pertanyaan penelitian yang diajukan. EDA membantu kami mendapatkan pemahaman awal tentang dataset dan menemukan wawasan yang mungkin tidak terlihat pada pandangan pertama. Kami fokus menjawab pertanyaan berikut:

#### 1. Pengaruh Ukuran Mesin Kendaraan terhadap Emisi CO2

Kami menjelajahi hubungan antara ukuran mesin kendaraan (Engine Size) dengan tingkat emisi CO2 (CO2 Emissions). Apakah kendaraan dengan mesin yang lebih besar cenderung memiliki emisi CO2 yang lebih tinggi?

#### 2. Hubungan Jumlah Silinder Mesin dan Emisi CO2

Kami menganalisis korelasi antara jumlah silinder mesin (Cylinders) dan emisi CO2 (CO2 Emissions). Apakah kendaraan dengan lebih banyak silinder cenderung menghasilkan emisi CO2 yang lebih tinggi?

#### 3. Dampak Jenis Transmisi pada Emisi CO2

Kami mengeksplorasi apakah jenis transmisi kendaraan (Transmission) memiliki dampak pada tingkat emisi CO2. Apakah jenis transmisi tertentu berkontribusi pada emisi CO2 yang lebih tinggi atau lebih rendah?

#### 4. Perbandingan Emisi CO2 antara Jenis Bahan Bakar

Kami membandingkan emisi CO2 antara kendaraan yang menggunakan jenis bahan bakar yang berbeda (Fuel Type). Apakah ada perbedaan signifikan dalam emisi CO2 antara kendaraan yang menggunakan jenis bahan bakar yang berbeda?

#### 5. Korelasi antara Efisiensi Bahan Bakar dan Emisi CO2

Kami mencari tahu apakah ada korelasi antara efisiensi bahan bakar, yang diukur dalam mil per galon (Fuel Consumption Comb (mpg)), dengan tingkat emisi CO2 (CO2 Emissions). Apakah kendaraan yang lebih efisien dalam penggunaan bahan bakar cenderung menghasilkan emisi CO2 yang lebih rendah?

#### 6. Hubungan antara Konsumsi Bahan Bakar per Mil dan Emisi CO2

Kami menganalisis hubungan antara konsumsi bahan bakar dalam mil per galon (mpg) dengan emisi CO2 (CO2 Emissions). Apakah ada pola yang dapat diidentifikasi dalam hubungan ini?

Analisis data eksploratori ini memberikan wawasan awal yang penting untuk merumuskan langkah-langkah berikutnya dalam proyek ini. Kami akan menggunakan temuan ini untuk membimbing langkah-langkah selanjutnya dalam mengembangkan model prediksi dan rekomendasi untuk mengurangi dampak lingkungan yang diakibatkan oleh emisi CO2.

## Pra-pemrosesan Data

Pada tahap ini, kami melakukan pra-pemrosesan data untuk memastikan bahwa data yang digunakan dalam pembangunan model Machine Learning adalah berkualitas dan relevan. Kami melakukan beberapa langkah penting seperti yang dijelaskan di bawah ini:

#### 1. Mengecek Nilai Null

Kami melakukan pemeriksaan terhadap nilai null atau missing values dalam dataset. Jika terdapat nilai null, kami akan mengidentifikasi apakah perlu menghapus baris atau mengisi nilai null dengan nilai lain yang sesuai.

#### 2. Handling Kategorik

Variabel kategorik seperti "Make", "Model", dan "Vehicle Class" mungkin memerlukan penanganan khusus. Kami akan menerapkan metode seperti one-hot encoding atau label encoding untuk mengubah variabel kategorik menjadi format yang dapat diterima oleh algoritma Machine Learning.

#### 3. Handling Numerik

Kami akan melakukan normalisasi atau standarisasi terhadap variabel numerik, seperti "Engine Size", "Cylinders", dan lainnya. Ini bertujuan untuk menghindari skala yang tidak seimbang antara variabel numerik yang berbeda, yang dapat mempengaruhi performa model.

Pra-pemrosesan data adalah langkah penting dalam persiapan data untuk model Machine Learning. Dengan melaksanakan langkah-langkah ini, kami dapat memastikan data yang digunakan dalam proses pembangunan model memiliki kualitas yang baik, sehingga model yang dihasilkan dapat memberikan hasil yang lebih akurat dan bermakna.

## Pembangunan dan Evaluasi Model

Dalam tahap ini, kami akan membangun model Machine Learning untuk memprediksi emisi CO2 berdasarkan variabel-variabel yang telah dijelaskan sebelumnya. Model yang kami pilih untuk proyek ini adalah Linear Regresi. Mengapa kami memilih Linear Regresi?

- Sederhana dan mudah diinterpretasi.
- Kecepatan dan efisiensi komputasi.
- Tidak terlalu sensitif terhadap overfitting.

#### Memilih Model Machine Learning

Setelah mempertimbangkan kelebihan Linear Regresi, kami memutuskan untuk menggunakannya sebagai model utama dalam proyek ini. Langkah selanjutnya adalah melatih model ini menggunakan data yang telah diproses.

#### Train-Test Split

Sebelum melatih model, kami perlu membagi dataset menjadi dua bagian: data latih (train data) dan data uji (test data). Dalam proyek ini, kami memilih perbandingan 70:30 untuk train data dan test data. Dengan memisahkan data ini, kami dapat melatih model pada data latih dan menguji performanya pada data uji yang belum pernah dilihat oleh model sebelumnya.

Langkah ini penting untuk memastikan bahwa model yang dibangun memiliki kemampuan yang baik dalam memprediksi data yang belum pernah dilihat sebelumnya. Hal ini membantu menghindari overfitting, di mana model terlalu "menghafal" data latih dan tidak dapat menggeneralisasi dengan baik pada data baru.

Dengan model Linear Regresi yang telah dilatih dan diuji pada data uji, kami dapat mengevaluasi performa model dan melihat sejauh mana model ini dapat memberikan prediksi yang akurat terhadap emisi CO2 berdasarkan variabel-variabel yang terlibat.

## Kesimpulan

Dalam analisis ini, kami telah melakukan serangkaian uji asumsi yang bertujuan untuk memeriksa kesesuaian model regresi dengan data yang telah dihadirkan. Berikut adalah ringkasan hasil dari setiap uji yang telah kami jalankan:

a. **Uji Linearitas**: Hasil analisis menunjukkan bahwa mayoritas variabel numerik memiliki hubungan positif dengan variabel target, dengan pengecualian variabel "fuel consumption mpg". Ini menggambarkan bahwa sebagian besar variabel numerik memainkan peran penting dalam mempengaruhi variabel target. Namun, perlu diperhatikan bahwa adanya hubungan non-linear pada variabel "fuel consumption mpg" mungkin memerlukan pendekatan analisis yang lebih cermat, mungkin dengan mempertimbangkan model non-linear atau transformasi.<br>

![Uji Indepedensi](https://github.com/hrmneffdi/-A-Data-Science-Exploration-CO2-Emissions/blob/main/uji_indepedensi.png)

b. **Uji Independensi**: Hasil menunjukkan bahwa plot residual tidak mengindikasikan pola tertentu, menggambarkan bahwa asumsi independensi antara residual terpenuhi. Hal ini menunjukkan bahwa setelah mempertimbangkan variabel independen, tidak ada tren atau pola yang jelas yang masih tersisa dalam residual.<br>

![Uji Homokedastisitas](https://github.com/hrmneffdi/-A-Data-Science-Exploration-CO2-Emissions/blob/main/uji_homokedastisitas.png)

c. **Uji Homoskedastisitas**: Pengamatan atas plot residual mengindikasikan adanya heteroskedastisitas, di mana variasi residual tidak merata di sepanjang rentang nilai prediksi. Fakta ini mungkin menunjukkan bahwa model regresi memiliki prediksi yang kurang konsisten dalam berbagai tingkat nilai prediksi. Untuk mengatasi hal ini, kami merekomendasikan eksplorasi lebih lanjut tentang faktor-faktor yang mungkin mempengaruhi variabilitas residual.<br>

![Uji Normalitas](https://github.com/hrmneffdi/-A-Data-Science-Exploration-CO2-Emissions/blob/main/uji_normalitas.png)

d. **Uji Normalitas**: Analisis terhadap distribusi residual mengindikasikan kemiripan dengan kurva normal, meskipun terdapat beberapa penyimpangan. Walaupun begitu, perlu diingat bahwa hasil ini lebih baik dikonfirmasi dengan uji statistik yang lebih khusus seperti uji Kolmogorov-Smirnov atau uji Shapiro-Wilk. Asumsi normalitas ini penting untuk dipenuhi guna memastikan validitas hasil analisis regresi.

e. **Uji Multikolinearitas**: Dari hasil perhitungan Variance Inflation Factor (VIF), kami menemukan bahwa semua variabel numerik memiliki nilai VIF lebih dari 10. Ini menunjukkan adanya tingkat multicollinearity yang signifikan antara variabel independen dalam model. Ketergantungan antar variabel ini dapat memengaruhi stabilitas koefisien regresi serta mempersulit interpretasi kontribusi individu dari setiap variabel.

Dalam kesimpulannya, model regresi yang telah dibangun mungkin telah memenuhi beberapa asumsi regresi seperti independensi dan normalitas. Meskipun demikian, terdapat beberapa area yang memerlukan perhatian, termasuk hubungan non-linear, heteroskedastisitas residual, dan multicollinearity yang signifikan. Kami merekomendasikan Anda untuk meninjau kembali proses pemilihan variabel, eksplorasi transformasi data, atau penerapan teknik analisis lainnya yang mungkin membantu mengatasi kendala ini. Dengan menyesuaikan model Anda, Anda dapat meningkatkan akurasi dan reliabilitas dalam meramalkan variabel target yang Anda minati.


## Terima Kasih
