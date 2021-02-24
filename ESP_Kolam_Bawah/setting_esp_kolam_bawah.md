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

6. Setelah flash tool terbuka, setting Port sesuai pada device manager tadi, pilih firmware(.bin) : blank_4Mb.bin --> pada saat pertama kali flash, sebaiknya flash terlebih dahulu menggunakan firmware blank agar semua file / konfigurasi pada wemos terhapus total. Setting baudrate 115.200 kemudian klik Flash untuk memulai proses flash :

