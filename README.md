# SmartHome Project dengan OpenHAB 3
 
Peralatan rumah kini dapat dikendalikan melalui internet karena telah disematkan teknologi Internet of Things(IoT). Untuk pengoperasiannya pemilik rumah harus memasang aplikasi yang telah dibuat oleh vendor ke smartphone miliknya. Ketika menggunakan banyak peralatan rumah dari vendor yang berbeda mengharuskan pemilik rumah menggunakan banyak aplikasi yang berbeda pula. Hal ini membuat pengendalian peralatan rumah menjadi tidak praktis karena harus berganti aplikasi setiap ingin mengendalikan peralatan rumahnya secara bergantian. 

Untuk mengatasi masalah diatas maka dirancanglah sebuah sistem smarthome dengan framework openHAB agar berbagai peratalan rumah saling terintegrasi dan dapat dikendalikan dengan satu aplikasi. OpenHAB adalah framework untuk smarthome yang bersifat opensource dan multiplatform. OpenHAB berperan sebagai sistem yang akan diterapkan pada raspberry pi. Informasi lengkap OpenHAB bisa diakses di website https://www.openhab.org/

Pertama kali, dilakukan konfigurasi jaringan internet rumah menggunakan provider Speedy serta menggunakan Mikrotik sebagai router jaringan utama sehingga peralatan yang terhubung ke jaringan baik melalui Wifi dan LAN akan ditangani oleh mikrotik.
 
 Topologi Jaringan :
![Home3](https://user-images.githubusercontent.com/73607420/109022827-c9828400-76ee-11eb-8ba4-eaeb4f6dc4fa.png)

Peralatan yang akan di integrasikan dengan OpenHAB adalah CCTV, lampu Teras / Balkon, Timer Controller System Flushing Filter Kolam Koi.

Konfigurasi masing-masing peralatan dapat dilihat pada folder masing - masing.

# DIY Timer Controller Filter Kolam Ikan Koi

Wiring Diagram :

![wemos pompa](https://user-images.githubusercontent.com/73607420/108999782-62a4a100-76d5-11eb-871b-d033a3fcc068.png)

Cara Kerja Alat :

Wemos D1 Mini sebagai kontroller untuk mengatur proses timer flushing filter kolam koi. Secara umum komunikasi antara Wemos D1 Mini dengan OpenHAB menggunakan HTTP Get Request & MQTT Protocol. OpenHAB akan mengirimkan perintah ke Wemos untuk menjalankan Rule melalui HTTP Get Request serta OpenHAB akan membaca status kondisi Pompa, Aerator dan Valve menggunakan Protokol MQTT.

![mqtt](https://user-images.githubusercontent.com/73607420/109001869-0e4ef080-76d8-11eb-9ede-bc23f0026119.png)

Cara konfigurasi Wemos D1 Mini :
