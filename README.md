Buat folder baru dengan nama lab11_ci pada docroot webserver (htdocs)
Sebelum memulai menggunakan Framework Codeigniter, perlu dilakukan konfigurasi pada webserver. Beberapa ekstensi PHP perlu diaktifkan untuk kebutuhan pengembangan Codeigniter 4. Berikut beberapa ekstensi yang perlu diaktifkan: • php-json ekstension untuk bekerja dengan JSON; • php-mysqlnd native driver untuk MySQL; • php-xml ekstension untuk bekerja dengan XML; • php-intl ekstensi untuk membuat aplikasi multibahasa; • libcurl (opsional), jika ingin pakai Curl.

Untuk mengaktifkan ekstentsi tersebut, melalu XAMPP Control Panel, pada bagian Apache klik Config -> PHP.ini
![Screenshot (168)](https://user-images.githubusercontent.com/56861575/122629132-02eb5f00-d0e5-11eb-9d72-c26a4c7fa0af.png)
Konfigurasi ekstensi PHP yang perlu diaktifkan seperti di gambar ini. Untuk mengaktifkan ekstensinya, hapus tanda ;
![Screenshot (159)](https://user-images.githubusercontent.com/56861575/122628945-8310c500-d0e3-11eb-9cf4-7adafac4061c.png)
![image](https://user-images.githubusercontent.com/56861575/122629170-5067cc00-d0e5-11eb-970e-6dd7afd6806a.png)


Untuk melakukan instalasi Codeigniter 4 dapat dilakukan dengan dua cara, yaitu cara manual dan menggunakan composer. Pada praktikum ini kita menggunakan cara manual. • Unduh Codeigniter dari website https://codeigniter.com/download • Extrak file zip Codeigniter ke direktori htdocs/lab11_ci. • Ubah nama direktory framework-4.x.xx menjadi ci4. • Buka browser dengan alamat http://localhost/lab11_ci/ci4/public/
![Screenshot (164)](https://user-images.githubusercontent.com/56861575/122629238-b6545380-d0e5-11eb-87b8-8a7e661bef5f.png)

Menjalankan CLI (Command Line Interface)
Perintah yang dapat dijalankan untuk memanggil CLI Codeigniter adalah: ( php spark )
![image](https://user-images.githubusercontent.com/56861575/122629276-0df2bf00-d0e6-11eb-8ec9-43c41a456747.png)

Ubah nama file env menjadi .env kemudian buka file tersebut dan ubah nilai variable CI_ENVIRINMENT menjadi development
![image](https://user-images.githubusercontent.com/56861575/122629447-48a92700-d0e7-11eb-8c45-3a3094882fd4.png)

Contoh error yang terjadi. Untuk mencoba error tersebut, ubah kode pada file app/Controller/Home.php hilangkan titik koma pada akhir kode.
![image](https://user-images.githubusercontent.com/56861575/122629487-958cfd80-d0e7-11eb-9d4e-ab0d7c9818ea.png)

Routing dan Controller
Router terletak pada file app/config/Routes.php
![image](https://user-images.githubusercontent.com/56861575/122629593-5ad79500-d0e8-11eb-81e2-ab6118bcb28e.png)

Selanjutnya coba akses route yang telah dibuat dengan mengakses alamat url http://localhost:8080/about
![Screenshot (164)](https://user-images.githubusercontent.com/56861575/122629711-3334fc80-d0e9-11eb-8c8b-f157e0f752ea.png)
Membuat Controller
Selanjutnya adalah membuat Controller Page. Buat file baru dengan nama page.php pada direktori Controller kemudian isi kodenya seperti berikut.
Selanjutnya refresh Kembali browser
![image](https://user-images.githubusercontent.com/56861575/122629832-11884500-d0ea-11eb-9600-a6d670be4c73.png)
![Capture10](https://user-images.githubusercontent.com/56861575/122629851-2e247d00-d0ea-11eb-8621-6a2f9107dfbe.JPG)

Buat file css pada direktori public dengan nama style.css
![Capture11](https://user-images.githubusercontent.com/56861575/122629889-4a281e80-d0ea-11eb-8cb4-0befa3a06a89.JPG)

Kemudian buat folder template pada direktori view kemudian buat file header.php dan footer.php
![footer](https://user-images.githubusercontent.com/56861575/122629912-6b890a80-d0ea-11eb-8076-37138d9c5466.JPG)
![header](https://user-images.githubusercontent.com/56861575/122629917-73e14580-d0ea-11eb-88df-c7a2d89dd7ca.JPG)

Kemudian ubah file app/view/about.php seperti berikut
![about](https://user-images.githubusercontent.com/56861575/122629943-9ecb9980-d0ea-11eb-9f5b-f9c19baafdfd.JPG)

tampilan akhir :
![image](https://user-images.githubusercontent.com/56861575/122629964-cd497480-d0ea-11eb-9274-abe47a2dd1e6.png)










