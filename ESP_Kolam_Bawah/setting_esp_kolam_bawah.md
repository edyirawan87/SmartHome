# Cara Setting ESP Kolam Bawah

Mikrokontroller yang dipakai disini menggunakan WEMOS D1 Mini serta firmware dari Easy ESP. Dokumentasi lengkap Firmware Easy ESP bisa di situs web : https://www.letscontrolit.com/wiki/index.php/ESPEasy

Alat & Bahan yang diperlukan :
  1. Wemos D1 Mini
  2. Firmware EasyESP (Cek di folder Firmware Easy ESP)
  3. Driver CH340 bisa di download di : https://www.wemos.cc/en/latest/ch340_driver.html
  4. Kabel USB micro

Langkah - langkah flash WEMOS D1 Mini menggunakan Firmware Easy ESP :

1. Download dan Ekstrak Firmware Easy ESP
2. Install Driver USB CH340
3. Hubungkan Wemos D1 Mini ke Komputer menggunakan USB
4. Setelah driver CH340 terinstal cek port wemos pada device manager :

![devmgmt](https://user-images.githubusercontent.com/73607420/109028436-6267ce00-76f4-11eb-86f3-8174a48f68cd.PNG)

5. Buka aplikasi flash Easy ESP :

![flash](https://user-images.githubusercontent.com/73607420/109028711-a955c380-76f4-11eb-8b74-f063a636f01d.PNG)

6. Setelah flash tool terbuka, setting Port sesuai pada device manager tadi, pilih firmware(.bin) : blank_4Mb.bin --> pada saat pertama kali flash, sebaiknya flash terlebih dahulu menggunakan firmware blank bertujuan agar semua file / konfigurasi pada wemos terhapus total serta memory pada wemos kembali Fresh. Setting baudrate 115.200 kemudian klik Flash untuk memulai proses flash :

![flash1](https://user-images.githubusercontent.com/73607420/109029885-dfe00e00-76f5-11eb-81bb-9bf1d280f206.png)

7. Setelah flash pertama menggunakan firmware blank_4Mb.bin selesai, flash kembali menggunakan firmware versi normal_ESP8266_4M1M.bin, tunggu sampai proses flashing selesai

![flash2](https://user-images.githubusercontent.com/73607420/109031066-f3d83f80-76f6-11eb-84f7-88cacde84e17.png)

8. Setelah proses flash selesai, lakukan reset wemos D1 Mini kemudian cek SSID Wifi dari wemos D1 Mini apakah sudah ada

![wifi](https://user-images.githubusercontent.com/73607420/109031665-82e55780-76f7-11eb-9dad-4229c83f5850.png)

9. Apabila proses flash berhasil, maka akan muncul SSID Wifi dari wemos D1 Mini dengan Nama : ESP-Easy
