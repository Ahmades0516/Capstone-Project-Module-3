# Capstone-Project-Module-3
Capstone project ini akan menganalisa Telco Churn Customer
# CONTENT
1. BUSINESS PROBLEMS
2. DATA UNDERSTANDING
3. MODELING
4. CONCLUTION AND RECOMMENDATION

# Business Problem Understanding

**Context**
Dalam dunia komersial, pelanggan adalah raja. Memahami pelanggan adalah hal yang paling penting dan memahami pola perilaku mereka dapat menghasilkan keputusan bisnis yang sangat berdampak. Customer Churn adalah tingkat di mana pelanggan komersial meninggalkan bisnis/platform komersial dan membawa uangnya ke tempat lain, dan memahami pola dasar pelanggan akan sangat memengaruhi kemampuan bisnis untuk mempertahankan pelanggannya. Sebagai seorang peneliti data yang mencoba masuk ke dunia profesional, menurut saya penting untuk mendapatkan pemahaman yang lebih baik tentang seperti apa fitur churn data ini dan bagaimana fitur tersebut dapat digunakan untuk memahami pelanggan.

Seorang Data Scientist diminta untuk membuat model prediksi yang tepat untuk menentukan pelanggan akan berhenti berlangganan (churn) atau tidak dengan menggunakan machine learning. 

Target :

1 : Berhenti berlangganan (churn)

0 : Tidak berhenti berlangganan


**Problem Statement:**

Banyak faktor yang mempengaruhi alasan seorang pelanggan melakukan Churn. Mungkin fakta bahwa ada pesaing baru di pasar yang menawarkan harga lebih baik atau mungkin layanan yang mereka dapatkan belum sesuai standar, dll.

Perusahaan telekomunikasi dapat memberikan insentif retensi seperti memberikan potongan harga, memberikan paket layanan yang menarik, memberikan
prioritas pelayanan dan lain-lain dalam upaya untuk mempertahankan pelanggan. Namun, kebijakan pemberian insentif retensi belum sepenuhnya dilakukan secara efektif. Karena jika insentif retensi tersebut diberikan secara merata kepada seluruh pelanggan, maka pengeluaran biaya tersebut menjadi tidak efektif dan mengurangi potensi keuntungan apabila pelanggan tersebut memang loyal dan tidak ingin berhenti berlangganan.

**Goals:**

Berdasarkan permasalahan tersebut, perusahaan ingin memprediksi pelanggan mana yang loyal dan akan churn berdasankan waktu tertentu. Hal ini sejalan untuk meningkatkan potensi keuntungan yang akan diperoleh perusahaan. Dan juga, perusahaan ingin mengetahui faktor-faktor apa saja yang cenderung mempengaruhi pelanggan bertahan, sehingga mereka dapat membuat program-program yang lebih tepat sasaran dalam mengurangi jumlah pelanggan yang churn. 

**Analytic Approach:**

Jadi yang akan kita lakukan adalah menganalisis data untuk menemukan pola yang membedakan pelanggan yang akan berhenti berlangganan (churn) atau tidak.

Kemudian kita akan membangun model klasifikasi yang akan membantu perusahaan untuk dapat memprediksi probabilitas seorang pelanggan akan berhenti berlangganan (churn) atau tidak. 

**Metric Evaluation**

Type 1 error : False Positive (pelanggan yang aktualnya tidak churn tetapi diprediksi churn)
Konsekuensi: tidak efektifnya pemberian insentif retensi

Type 2 error : False Negative (pelanggan yang aktualnya churn tetapi diprediksi tidak akan churn)
Konsekuensi: kehilangan pelanggan

Berdasarkan konsekuensinya, maka hal terbaik yang dapat dioptimasikan yaitu meminimalkan biara yang dikeluarkan untuk penawaran khusus untuk pelanggam tetapi juga tidak membuat pelanggan menjadi churn/tidak berlangganan lagi. Maka metric yang cocok untuk hal ini adalah recall  yaitu memaksimalkan nilai **Recall/True Positive Rate** dan meminimalkan **False Negatif**. Hal ini sama dengan mengoptimalkan nilai recall, sehinggan recall menjadi parameter kunci dalam kasus ini
