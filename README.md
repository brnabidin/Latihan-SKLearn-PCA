# Latihan-SKLearn-PCA

Tahapan pada latihan ini sebagai berikut:

- Bagi dataset.

- Latih model tanpa PCA.

- Latih model dengan PCA.

- Evaluasi hasil kedua model.

# Codelab 

Pada Colaboratory impor library yang dibutuhkan.  Kemudian kita masukkan dataset iris dan bagi data menjadi train set dan test set.

![1](https://github.com/brnabidin/Latihan-SKLearn-PCA/assets/67081096/181801ae-dc1c-46d5-8332-8241ae342a85)

Kita akan menggunakan model Decision Tree dan menghitung berapa akurasinya tanpa menggunakan PCA. Akurasi tanpa PCA adalah 0.9666. Akurasi dari model Anda mungkin berbeda dengan keluaran di bawah.

![2](https://github.com/brnabidin/Latihan-SKLearn-PCA/assets/67081096/f95fae38-740f-4a4e-bac8-0a3063650f27)

Tampilan hasil akurasi tanpa PCA dari kode di atas sebagai berikut.

![20200430230236955611691969fb031f6be6d185d902ae](https://github.com/brnabidin/Latihan-SKLearn-PCA/assets/67081096/58b3c8d3-a3a9-4bd9-8238-c837365d8a21)

Kemudian kita akan menggunakan PCA dan menghitung variance dari setiap atribut. Hasilnya adalah 1 atribut memiliki variance sebesar 0.922, yang berarti atribut tersebut menyimpan informasi yang tinggi dan jauh lebih signifikan dari atribut lain. 

![3](https://github.com/brnabidin/Latihan-SKLearn-PCA/assets/67081096/d0dc7704-3dd8-4b5b-ba45-7e4aa3ad2ef4)

Hasil dari setiap atributnya menjadi sebagai berikut.

![202004302306411f9b2237edc16045f4f6a31d7f0183a9](https://github.com/brnabidin/Latihan-SKLearn-PCA/assets/67081096/8805ece1-e86f-46d9-a89d-339882d98c81)

Melihat dari variance sebelumnya kita bisa mengambil 2 principal component terbaik karena total variance nya adalah 0.976 yang sudah cukup tinggi.

![4](https://github.com/brnabidin/Latihan-SKLearn-PCA/assets/67081096/624e7df4-19dd-40bb-8502-902ef429fcdc)

Kita akan menguji akurasi dari classifier setelah menggunakan PCA.

![5](https://github.com/brnabidin/Latihan-SKLearn-PCA/assets/67081096/2cda0e23-9f3b-49c0-a7fa-ec5bf090365f)

Hasil pengujian akurasi setelah menggunakan PCA menjadi seperti di bawah ini.

![20200430231028ae2b75175eb26e463eb621d984a237fc](https://github.com/brnabidin/Latihan-SKLearn-PCA/assets/67081096/d47c3a7a-e77c-4227-a648-804c625db74c)

Dari percobaan di atas bisa kita lihat bahwa dengan hanya 2 principal component atau 2 atribut saja model masih memiliki akurasi yang tinggi. Dengan principal component kamu bisa mengurangi atribut yang kurang signifikan dalam prediksi dan mempercepat waktu pelatihan sebuah model machine learning.
