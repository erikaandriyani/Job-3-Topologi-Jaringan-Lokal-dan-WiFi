# Topologi-Jaringan-Lokal-dan-WiFi

Wireless Fidelity atau yang lebih awam kita sebut wifi adalah suatu teknologi yang menggunakan gelombang radio dalam rentang 2,4GHz sampai dengan 5GHz untuk menghubungkan perangkat seperti PC/laptop, smartphone, dan perangkat microcontroller seperti ESP32 dan ESP8266 ke jaringan lokal wireless untuk bisa mengakses internet. Untuk dapat melakukan akses internet tersebut,maka perangkat elektronik diatas perlu berada dalam satu titik akses atau hotspot jaringan nirkabel sehingga terhubung dengan wifi. Pada umumnya jaringan wifi dapat menjangkau hingga 20 meter didalam ruangan dan lebih dari 20 meter untuk di luar ruangan. Pada awal kemunculannya, wifi hanya digunakan sebagai perangkat nirkabel pada jaringan LAN (Local Area Network) akan tetapi karena pesatnya teknologi di zaman sekarang wifi menjadi kebutuhan sehari-hari untuk akses jaringan internet dan IoT.

**ALAT DAN BAHAN**
1) ESP32
2) Breadboard
3) Kabel jumper
4) Sensor DHT 11, RFID
5) LED (5) dan Push Button (3)
6) Servo
7) Resistor 330,1K, 10K Ohm (@ 3)

**HASIL KELUARAN**

**1) ESP32 WiFi Modes dan WiFi Scan**
![ESP32 Wifi dan Wifi Scan](https://user-images.githubusercontent.com/118364435/206267667-efbd1894-a570-4f84-979f-c742f35a85d7.jpeg)

Analisa : Percobaan ini adalah percobaan untuk men-scan WiFi yang ada di sekitar. Sperti pada keluaran, setelah script di run, maka serial monitor akan menampilkan data semua WiFi yang bisa dijangkau oleh ESP32.

**2) Menghubungkan ESP32 Dengan Jaringan WiFi**
![Menghubungkan ESP32 dengan jaringan Wifi](https://user-images.githubusercontent.com/118364435/206267866-c2d1cf68-6645-496e-bfac-645e2acbb1b7.jpeg)

Terhubung ke Perangkat

![Menghubungkan ESP32 dg jar Wifi (di prngkt)](https://user-images.githubusercontent.com/118364435/206267934-21705c35-99d1-4c60-9817-bea080831f07.jpg)

Analisa : Percobaan ini adalah menghubungkan ESP32 dengan WiFi, dan kami menggunakan WiFi dari andrioid dengan hostname HernaningErika. Namun sebelumnya, isi lebih dulu SSID dan password WiFi pada script untuk mendeteksi WiFi tersebut. Jika script dirun dan tersambung WiFi, pada serial monitor akan tertulis Connecting to WiFi dan tertera juga alamat IP dari WiFi tersebut. Jika sudah seperti ini, maka ESP32 tersambung ke WiFi tersebut. Seperti pada tampilan keluaran di atas melalui android, esp32-arduino terhubung dengan WiFi dari android tersebut.

**3) Re-Connect ESP32 Dengan Jaringan WiFi**
![Reconnecting ESP32 dengan jaringan Wifi](https://user-images.githubusercontent.com/118364435/206268095-17bf0158-dfd2-438a-81fd-a397b92cfa2d.jpeg)

Re-Connect di Perangkat

![Reconnecting ESP32 (di perangkat)](https://user-images.githubusercontent.com/118364435/206268172-a912f9f2-3c7c-417b-9040-1e7647a1bd1d.jpg)

Analisa : Di percobaan ini diinginkan agar ESP32 Re-connect ke WiFi. Dengan menggunakan WiFi yang sama, hubungkan ESP32 dengan WiFi. Jika sudah terhubung, coba matikaN WiFi untuk sesaat. Jika Wifi dinyalakan kembali dan serial menampilkan Re-connecting, maka ESP32 sedang menyambungkan ulang ke WiFi tersebut. Dan pada android akan tersambung kembali.

**4) Mengganti Hostname ESP32**
![Mengganti hostname ESP32 (tampilan serial monitor)](https://user-images.githubusercontent.com/118364435/206268306-5ba1a6fe-9773-4de9-9ecf-f14e7326e96a.jpeg)

Hostname Berubah di Perangkat

![Mengganti hostname ESP32 (tmpilan di prngkat wifi)](https://user-images.githubusercontent.com/118364435/206268409-1171089b-2276-4613-aba2-134b094c9957.jpg)

Analisa : Pada percobaan ini diminta untuk mengganti nama hostname ESP32. Yang sebelumnya bernama esp32-arduino, kali ini diubah menjadi ESP32. Ketika script dirun, maka hostname akan berubah menjadi ESP32, bisa dicek juga pada android (perangkat). Namun jika pada saat run, hostname belum berubah, lakukan uploaing ulang atau ganti nama hostnamenya.

**5) Mengirim Data Sensor ke Database**

![Rangkaian Bagus Mengirim data sensor DHT11 ke database](https://user-images.githubusercontent.com/118364435/206268814-c46caf34-e980-41c7-805d-b7c781c5dbad.jpeg)

Keluaran (Untuk Mengetahui IP Address di Serial Monitor)
![Mengirim data sensor DHT11 ke database (serial monitor)](https://user-images.githubusercontent.com/118364435/206269071-ff10ba9a-b5b0-4646-aa96-ef24f8e9641d.jpeg)

Keluaran (Akses IP Address di Web Browser)
![Mengirim data sensor DHT11 ke database (web browser)](https://user-images.githubusercontent.com/118364435/206269197-c0bf2a38-06f9-42be-bb2d-ec2a634e4d35.jpeg)

Analisa :
