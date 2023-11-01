# Project AI-KMMI-Mask-Detection

### Penjelasan
Pada percobaan ini menggunakan dataset yang terdiri dari data train dan data validasi masing-masing data tersebut memiliki 2 kelas yaitu with_mask dan without_mask. Untuk data train terdiri dari 3833 gambar dan data validasi terdiri dari 616 gambar. Namun saya hanya menggunakan 2000 gambar sampel untuk data train dan 400 gambar sampel untuk data validasi. Untuk proses training saya mencoba menggunakan epoch 10 dan nilai batch size 64. Berikut ini gambar dari proses training :

![image](https://github.com/Rifqiakmals12/Project-2-KMMI-Mask-Detection-Using-Transfer-Learning/assets/72428679/eaae58e9-5c43-49fb-9306-a69d2d28c54d)

Gambar 1.1 Hasil Training

Berdasarkan gambar diatas pada epoch ke-5 mendapatkan model face_recognition.h5 terbaik dengan hasil loss: 0.0299 - accuracy: 0.9869 - val_loss: 0.0069 - val_accuracy: 1.0000 setelah itu dari epoch ke 6-10 tidak ada peningkatan dari val_loss nya. Jadi dapat disimpulkan model face_recognition.h5 pada epoch ke-5 akan disimpan dan digunakan untuk proses deteksi masker. Berikut ini merupakan gambar grafik akurasi training dan validasi, nilai loss training dan validasi, confusion matrix dan hasil klasifikasi.
 
 
![image](https://github.com/Rifqiakmals12/Project-2-KMMI-Mask-Detection-Using-Transfer-Learning/assets/72428679/87afce3c-3cfa-49dc-90d8-9552e04d0f71)

Gambar 1.2 Training dan Validation Accuracy


![image](https://github.com/Rifqiakmals12/Project-2-KMMI-Mask-Detection-Using-Transfer-Learning/assets/72428679/d8d087eb-5632-4798-bdb3-a600a743ae84)

Gambar 1.3 Training and Validation Loss


![image](https://github.com/Rifqiakmals12/Project-2-KMMI-Mask-Detection-Using-Transfer-Learning/assets/72428679/357dd86e-5349-4675-9659-4d3fa377c7b3)

Gambar 1.4 Confusion Matrix dan Hasil Klasifikasi
 
Berikut ini hasil running dari program Real-time Video yang menggunakan hasil model face_recognition.h5 :

![image](https://github.com/Rifqiakmals12/Project-2-KMMI-Mask-Detection-Using-Transfer-Learning/assets/72428679/bd4833ee-1f70-4d63-93c1-fe5791c7909e)

Gambar 1.5 Hasil Saat Menggunakan Masker


![image](https://github.com/Rifqiakmals12/Project-2-KMMI-Mask-Detection-Using-Transfer-Learning/assets/72428679/38508529-941b-42df-9b73-81cf700023ed)

Gambar 1.6 Hasil Saat Tidak Menggunakan Masker


