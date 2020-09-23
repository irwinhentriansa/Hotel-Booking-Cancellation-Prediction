#  ``Hotel Reservation Cancellation Prediction``

Dataset berisi informasi pemesanan kamar hotel (*booking information*) baik untuk hotel kota (*city hotel*) maupun hotel resort. Dataset ini juga mengandung kapan *booking* dilakukan, lama menginap, jumlah pengunjung dewasa, anak-anak, dan/atau bayi, serta ketersediaan tempat parkir. Informasi lain mengenai dataset bisa Anda baca di keterangan dataset di bawah ini:

## **Dataset**

Dataset ini berasal dari paper Jurnal Ilmiah berjudul "Hotel booking demand datasets" yang ditulis oleh Nuno Antonio, Ana Almeida, and Luis Nunes for Data in Brief, Volume 22, February 2019. Penjelasan tiap feature/variabel dari Jurnal bisa Anda akses di  https://www.sciencedirect.com/science/article/pii/S2352340918315191

Apabila kesulitan download dataset pada repo ini atau ingin mengetahui keterangan di setiap kolom, bisa akses ke: https://www.kaggle.com/jessemostipak/hotel-booking-demand/data. 

### **A. Data Cleaning & Preprocessing**

__Batasan Data:__
* __Ukuran data__ yang digunakan adalah 5000 baris (_rows_) awal [:5000].
* __Variabel__ yang dipakai berjumlah 16 kolom, yaitu: ['hotel', 'is_canceled', 'adults', 'children', 'babies', 'meal', 'country', 'market_segment', 'distribution_channel', 'reserved_room_type', 'booking_changes', 'deposit_type', 'days_in_waiting_list', 'customer_type', 'required_car_parking_spaces', 'total_of_special_requests']

### **B. EDA** 
Membuat Exploratory Data Analysis untuk:
1) Memahami profil tamu/konsumen hotel (_customer profiling_).
2) Memahami kebiasaan tamu/konsumen hotel (_customer behavior_).

### **C. Model Building & Hyper-parameter Tuning** 
1) Melakukan _training_ 3  model ML. Untuk mendapatkan model ML terbaik untuk memprediksi apakah user akan *cancel booking* atau tidak! 

2) Menjelaskan secara singkat cara kerja model ML yang digunakan!

3) Meningkatkan performa model ML mengikuti instruksi *model evaluation*. 

### **D. Model Evaluation**
Ada **2 jenis kesalahan** yang mungkin terjadi dalam model ML di studi kasus ini, yaitu:
1. Model memprediksi user akan *cancel booking* (membatalkan pesanan), padahal sebenarnya/realisasinya user tidak membatalkan pesanan.
2. Model memprediksi user tidak membatalkan pesanan, padahal sebenarnya/realisasinya user *cancel booking* (membatalkan pesanan).

Dalam konteks bisnis perhotelan, apabila pengunjung diasumsikan tidak *cancel booking* maka pihak hotel akan menyiapkan beberapa hal untuk menyambut kedatangan mereka, di antaranya:
1. Menghubungi pengunjung terkait kapan perkiraan datang ke hotel,
2. Membersihkan, merapikan, dan menyiapkan kamar sesuai pesanan pengunjung,
3. Menyiapkan makanan dan minuman untuk menyambut kedatangan pengunjung,
4. Menolak pengunjung lain yang memesan kamar yang telah dipesan (*booked room*), dan
5. Memberi layanan penjemputan di bandara/stasiun/terminal apabila diperlukan.
