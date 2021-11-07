# Assignment-1-DDP
A file that summarizes which problems you can solve, each blessing, and a total blessing.

# Linear Congruential Generator
Salah satu Pembangkit bilangan acak Semu atau Pseudo Random Number Generator (PRNG) sebagai dasar yang cukup baik untuk dipelajari adalah Linear Congruential Generator (LCG) dengan rumus:

Xn = (a * Xn – 1 + b) % m

Dimana:

Xn = bilangan acak ke-n dari deretnya

Xn – 1 = bilangan acak sebelumnya

a = faktor pengali

b = increment

m = modulus pembagi

Untuk permulaan, dibutuhkan X0 sebagai kunci pembangkit untuk mengenerate kunci-kunci selanjutnya (X0, X1, X2, X3 dan seterusnya).  X0 disebut sebagai umpan atau seed. Dalam membangkitkan angka random, metode LCG mempunyai periode pengulangan yang kurang dari m (modulus pembagi). Perhatikan hasil running di atas. Pembagi modulus diisi 11, sehingga LCG mampu men-generate angka random dari deret ke-0 sampai ke-10, ketika memasuki periode ke-11 proses akan berulang menampilkan nilai yang sama dengan nilai sebelumnya  (X0, X1, X2, X3 sampai X11). 

Suatu LCG mempunyai periode penuh (m – 1) jika memenuhi syarat sebagai berikut:

b relatif prima terhadap m.

a – 1 dapat dibagi dengan semua faktor prima dari m

a – 1 adalah kelipatan 4 jika m adalah kelipatan 4

m > maks(a, b, X0)

a > 0

b > 0

LCG memiliki kelebihan pada kecepatannya karena sedikit  membutuhkan operasi bit namun urutan kemunculan bilangan acaknya, mudah diprediksi sehingga tidak aman secara kriptografi. Namun demikian, LCG tetap berguna untuk latihan awal penerapan enkripsi dengan metode stream cipher menggunakan kunci yang dibangkitkan oleh algoritma LCG. Selain itu LCF dapat diterapkan pada aplikasi simulasi lain karena algoritma ini sangat mangkus (efisien secara waktu proses dan hemat penggunaan memory).
