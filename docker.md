1. Jelaskan apa yang dimaksud dengan container pada docker !

Wadah untuk mengemas dan menjalankan aplikasi. Wadah ini berisi kode, waktu proses, alat sistem, dan pengaturan. Wadah hanya dapat mengakses sumber daya yang ditentukan dalam gambar Docker. Wadah ini berperilaku seperti mesin virtual yang berjalan seperti simulasi komputer di komputer nyata pengembang. Mesin virtual ini berisi semua kode sistem untuk menjalankan simulasi seolah-olah itu adalah operasi sistem utama. Docker digunakan untuk memvirtualisasikan sistem operasi dalam sistem operasi host. Docker membuat wadah berdasarkan image yang berisi kode program. image ini ditumpuk di atas satu sama lain untuk membentuk keselarasan yang sempurna.

2. Jelaskan apa perbedaan antara konsep container dengan virtual machine !

- VM memakan banyak resource dan waktu utk booting karena melakukan virtualisasi pada host hardware-nya, container melakukan virtualisasi pada host OS-nya.

- VM hanya dapat berjalan pada hypervisor. Sedangkan Container tidak.

- VM menggunakan kernel tersendiri untuk menjalankan aplikasi didalamnya. Sedangkan container tidak diizinkan untuk mengakses kernel.

- VM adalah software yang memungkinkan untuk mengisolasi sebuah mesin komputer serta dapat menjalankan semua program yang sama seperti pada komputer aslinya atau biasa disebut duplikat dari sebuah mesin komputer asli. Sedangkan, Container dalam bahasa komputer adalah suatu teknologi yang dapat mengisolasi sebuah proses dari proses yang lainnya yang akan mengisolasi library dan aplikasi yang digunakan saja tanpa mengisolasi seluruh komponen seperti perangkat keras, kernel, sistem operasi, dan lain - lain.

3. Apa yang dimaksud dengan docker file ?
   Docker file adalah dokumen teks yang berisi semua perintah yang dapat dipanggil pengguna pada baris perintah untuk merakit gambar. Menggunakan docker build pengguna dapat membuat build otomatis yang mengeksekusi beberapa instruksi baris perintah secara berurutan.

4. Apa yang dimaksud dengan docker registery ?
   Docker registery adalah penyimpanan dan distribusi sistem bernama Docker gambar. Gambar yang sama mungkin memiliki beberapa versi berbeda, yang diidentifikasi oleh tagnya.

5. Jelaskan bagaimana cara untuk menjalankan lebih dari 1 container secara bersamaan dan saling terhubung !
   Docker-Compose adalah alat untuk mendefinisikan dan menjalankan satu atau beberapa container yang saling terkait dengan sebuah command.

Caranya:

1. Buat file NAMA_FILE.yaml di dalam project yang kamu buat
2. Tulis beberapa perintah ke dalam sana
3. Buat Dockerfile pada masing-masing project yang ingin digabung
4. Jalankan menggunakan perintah
   docker-compose NAMA_FILE.yaml up
