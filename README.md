# HR-Performance-Analytics-Jaya-Jaya

# Proyek Akhir: Menyelesaikan Permasalahan Attrition Rate Perusahaan Jaya Jaya Maju 

## Business Understanding

Jaya Jaya Maju merupakan salah satu perusahaan multinasional yang telah berdiri sejak tahun 2000. Ia memiliki lebih dari 1000 karyawan yang tersebar di seluruh penjuru negeri. 

Walaupun telah menjadi menjadi perusahaan yang cukup besar, Jaya Jaya Maju masih cukup kesulitan dalam mengelola karyawan. Hal ini berimbas tingginya attrition rate (rasio jumlah karyawan yang keluar dengan total karyawan keseluruhan) hingga lebih dari 10%.

Untuk mencegah hal ini semakin parah, manajer departemen HR ingin mengidentifikasi berbagai faktor yang mempengaruhi tingginya attrition rate tersebut. Selain itu, ia juga meminta untuk membuat business dashboard untuk membantunya memonitori berbagai faktor tersebut.

### Permasalahan Bisnis

1. Identifikasi faktor-faktor apa saja yang mempengaruhi tingginya attrition rate di perusahan Jaya Jaya Maju
2. Pembuatan Dashboard Untuk Membantu HR memonitor attrition rate 
3. Membuat model machine learning yang dapat membantu HR dalam memprediksi kemungkinan attrition rate/karyawan yang attrition di perusahaan tersebut

### Cakupan Proyek

Pertama-tama yaitu untuk mengidentifikasi faktor-faktor apa aja yang mempengaruhi tingkat attrition di perusahaan tersebut, lalu membuat business dashboard yang dapat membantu tim HR untuk monitoring attrition rate di perusahaan tersebut, lalu membuat model machine learning (random forest) yang dapat membantu tim HR untuk memprediksi apakah karyawan akan attrition dari perusahaan tersebut atau tidak, kemudian memberikan rekomendasi untuk tim HR yang dapat membantu untuk mengurangi tingkat attrition rate di perusahaan tersebut. 

### Persiapan

Sumber data: https://github.com/dicodingacademy/dicoding_dataset/tree/main/employee
Setup environment:


Set Up Environment Anaconda

conda create --name hr-analytics python=3.11.12
conda activate hr-analytics
pip install -r requirements.txt

Set Up Environment Shell/Terminal

mkdir hr-analytics
cd hr-analytics
pipenv install
pipenv shell
pip install -r requirements.txt

File:
random_forest_model.joblib
→ Model Random Forest yang telah dilatih.

prediction.py
→ Script Python untuk menjalankan proses prediksi dengan model.



## Business Dashboard

Business dashboard ini bertujuan untuk membantu HR perusahaan Jaya Jaya Maju dalam memonitor tingkat attrition rate di perusahaan, dashboard ini memuat faktor-faktor yang mempengaruhi tingkat attrition rate di perusahaan Jaya Jaya Maju, diantaranya itu tingkat attrition berdasarkan business travel, Jarak dari rumah karyawan ke kantor, gaji bulanan karyawan, Job level, Age Group, Job Involvement, Departemen, tingkat Pendidikan, status pernikahan, job role. Pada beberapa variable, saya membaginya atau mengelompokkannya menjadi beberapa bagian agar mudah mendapatkan insightnya. Dari total 1058 karyawan, tingkat attrition ratenya 16.92%, dengan rata-rata gaji bulanan karyawannya sekitar 6,63k USD, rata-rata karyawan bekerja selama 7 tahun, dan rata-rata usia karyawan 37 tahun. Tingkat attrition paling tinggi berdasarkan bisnis travel ada pada karyawan yang jarang melakukan perjalanan bisnis sekitar 117 orang, karyawan yang memiliki job level rendah cenderung memiliki tingkat attrition yang tinggi, juga karyawan yang memiliki gaji bulanan rendah juga tingkat attrition ratenya tinggi, departemen yang paling tinggi tingkat attrition ratenya adalah departemen Research & Development sekitar 59% dan terendah pada departemen HR hanya sekitar 3.4 %, karyawan yang memiliki Jarak rumah jauh dari kantor juga tingkat attrition nya tinggi, lalu karyawan generasi Gen Y dan Gen Z merupakan generasi yang memiliki tingkat attrition rate tinggi dibandingkan generasi lainnya di perusahaan Jaya Jaya Maju, karyawan yang masih single tingkat attrition ratenya paling tinggi dibandingkan karyawan yang sudah menikah atau bercerai, Karyawan laki-laki di perusahaan Jaya-Jaya Maju lebih tinggi attritionnya dibandingkan aryawan perempuannya yaitu 108 karyawan berabnding dengan 71 karyawan, Job Role Technician Laboratory dan Research Scientist tingkat attritionnya paling tinggi diantara job role lainnya. 

Link: https://lookerstudio.google.com/reporting/0056a74d-4261-41d6-be74-a7cac4def734

## Conclusion

Tingkat attrition rate perusahaan Jaya-Jaya Maju dipengaruhi oleh beberapa faktor yaitu tingkat attrition berdasarkan business travel, Jarak dari rumah karyawan ke kantor, gaji bulanan karyawan, Job level, Age Group, Job Involvement, Departemen, tingkat Pendidikan, status pernikahan, job role. Namun, yang paling berpengaruh menurut aya adalah pada tingkat gaji karyawan, job level, job role, Jarak rumah ke kantor, dan status pernikahan. Saya juga melakukan penerapan model mesin learning untuk membantu HR untuk mengatasi masalah ini, yaitu dengan model random forest, akurasi yang saya peroleh yaitu sekitar 88%.

### Rekomendasi Action Items (Optional)

Berikan beberapa rekomendasi action items yang harus dilakukan perusahaan guna menyelesaikan permasalahan atau mencapai target mereka.

- Meningkatkan gaji karyawan mereka
- Mengevaluasi departemen yang paling banyak tingkat attrition ratenya, yaitu R&D untuk mengetahui permasalahan yang menjadi faktor mereka attrition dari perusahaan mereka.
