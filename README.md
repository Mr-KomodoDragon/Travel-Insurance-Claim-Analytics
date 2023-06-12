# **Travel Insurance Claim Analytics**

### **Created By: Joel Bernard Leonardo**
## **Business Problem Understanding**

**Context**: <br>
Asuransi perjalanan adalah jenis asuransi yang memberikan perlindungan selama kita melakukan perjalanan baik di dalam negeri maupun ke luar negeri. Beberapa negara bahkan mensyaratkan para pelancong untuk memiliki asuransi perjalanan, contohnya di negara-negara Eropa dan Amerika. Jumlah premi yang harus dibayarkan tergantung pada cakupan yang diinginkan, durasi perjalanan, dan tujuan perjalanan. Sebuah perusahaan yang bergerak di bidang asuransi perjalanan ingin mengetahui calon pemegang polis yang akan mengajukan klaim asuransi untuk mendapatkan perlindungan. Data pemegang polis di perusahaan asuransi adalah data historis yang mencakup tujuan perjalanan, produk asuransi, dan lain-lain

(Note: Perusahaan Travel Asuransi ini menawarkan Asuransinya lewat pihak ketiga)


**Target**:<br>
0 : Tidak mengajukan klaim asuransi

1 : mengajukan klaim asuransi


**Problem Statement** :<br>
Perushaan ingin  meningkatkan efisiensi proses klaim asuransi perjalanan dengan memanfaatkan data historis pemegang polis untuk mengidentifikasi pemegang polis yang berpotensi mengajukan klaim dan membutuhkan perlindungan, sehingga dapat mengoptimalkan sumber daya perusahaan. Perusahaan menawarkan asuransinya lewat pihak ketiga kepada setiap orang akan tetapi hal itu membuat rugi perusahaan, karena perusahaan tidak mengetahui apakah orang yang ditawarkannya akan klaim atau tidak.


**Goals** :<br>
Maka berdasarkan permasalahan tersebut, perusahaan ingin memiliki kemampuan untuk memprediksi kemungkinan calon pemegang polis akan mengajukan klaim atau tidak. Sehingga tidak akan merugikan finasial perushaan Travel Insurance, karena Perushaan akan mengetahui calon pemegang polis tersebut dipastikan tidak akan klaim.

**Analytic Approach** :<br>
Jadi yang akan saya lakukan adalah menganalisis data untuk menemukan pola yang membedakan orang pemegang polis akan klaim atau tidak (klasifikasi).

Kemudian saya akan membangun model klasifikasi yang akan membantu perusahaan untuk dapat memprediksi probabilitas seorang akan klaim asurasi tersebut atau tidak.

**Metric Evaluation**

![Metric_eva.png](https://github.com/Mr-KomodoDragon/ML-Travel-Insurance/blob/main/Metric_eva.png?raw=true)

Type 1 error : False Positive,<br>
Model memprediksi Cutomer akan klaim tapi kenyataan tidak, maka perusahaan kehilangan calon customer mereka. Karena mereka tidak ditawarkan.

Type 2 error : False Negative,<br>
Model memprediksi Customer akan tidak klaim tapi kenyataan iya, maka perusahaan rugi karena harus memberi uang klaim kepada customer tersebut.

Berdasarkan Permintaan Perusahaan, saya akan membuat model yang dapat mengidetifikasi customer yang memegang polis yang akan Claim. Dan dari konsekuensi bahwa keduanya sangat penting maka dari itu saya akan fokus terhadap False Negative lebih dari False Postive, tapi tetap memperhatikan keduanya. Maka Metric utama yang saya gunakan adalah **f2**.

Note:
- f2 : recall (FN) lebih penting dari pada precision (FP), tapi tetap memperhatikan keduanya.

