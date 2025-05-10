# Kelompok-IOT
kelompok 6
🔩 Alat dan Bahan

🔌 Elektronik:

1.	1x Arduino UNO (bisa juga pakai NodeMCU atau Arduino Nano)

2.	1x Sensor DHT11 (modul atau sensor biasa)

3.	1x Breadboard

4.	3x LED:

o	1x LED Hijau

o	1x LED Kuning

o	1x LED Merah


5.	3x Resistor 220 ohm (untuk membatasi arus ke LED)

6.	1x Resistor 10k ohm (jika pakai DHT11 tanpa modul – sebagai pull-up resistor)

7.	Kabel jumper secukupnya

8.	Kabel USB untuk menghubungkan Arduino ke komputer

 

🧰 Alat Pendukung:

1.	Laptop/PC dengan Arduino IDE terinstal

2.	Multimeter (opsional, untuk mengecek koneksi)

3.	Tang potong/kabel (jika perlu)

4.	Papan kerja atau tatakan (jika ingin lebih rapi)


🧪 Tata Cara Praktik

1.	Persiapan:

o	Pasang semua komponen pada breadboard sesuai dengan diagram koneksi di atas.



Koneksi Rangkaian:

DHT11:

- VCC    → 5V pada Arduino

- DATA   → Pin D2 pada Arduino

- GND    → GND pada Arduino


LED Hijau:

- Anoda (+) → Pin D5 pada Arduino melalui resistor 220Ω

- Katoda (–) → GND pada Arduino


LED Kuning:

- Anoda (+) → Pin D6 pada Arduino melalui resistor 220Ω

- Katoda (–) → GND pada Arduino


LED Merah:

- Anoda (+) → Pin D7 pada Arduino melalui resistor 220Ω

- Katoda (–) → GND pada Arduino



Catatan: Jika Anda menggunakan sensor DHT11 tanpa modul, tambahkan resistor pull-up 10kΩ antara pin VCC dan DATA.

o	Hubungkan Arduino ke komputer menggunakan kabel USB.


2.	Instalasi Library:

o	Buka Arduino IDE.

o	Masuk ke menu Sketch > Include Library > Manage Libraries...

o	Cari "DHT sensor library" oleh Adafruit dan instal.Arduino Project Hub+1techZeero+1

3.	Unggah Kode: 

o	Tempelkan ke dalam Arduino IDE.

o	Klik tombol Upload untuk mengunggah kode ke Arduino.

4.	Pengujian:

o	Buka Serial Monitor dengan baud rate 9600 untuk melihat data suhu dan kelembaban.

o	Amati perubahan pada LED sesuai dengan suhu yang terbaca.Instructables

 

**💡 Tips Tambahan**

•	Untuk pengujian, Anda dapat memanaskan sensor dengan tangan atau meniupkan udara hangat untuk melihat perubahan pada LED.





🧠 Penjelasan Fungsi

Program Arduino ini membaca suhu dan kelembaban dari sensor DHT11. Berdasarkan nilai suhu yang terbaca, program mengontrol tiga LED sebagai indikator:

•	LED Hijau menyala jika suhu < 25°C (suhu dingin).

•	LED Kuning menyala jika suhu antara 25°C hingga 30°C (suhu normal).

•	LED Merah menyala jika suhu > 30°C (suhu panas).

Data suhu dan kelembaban juga ditampilkan pada Serial Monitor setiap 2 detik.



Kegunaan:

Cocok untuk proyek monitoring suhu ruangan atau lingkungan, seperti:

•	Ruangan server,

•	Greenhouse (rumah kaca),

•	Kamar anak/bayi,

•	Ruang penyimpanan makanan.

Berikut link video praktik kami:

https://youtu.be/z4TdQpXGIig?si=ce2w6wdmp5rxQ7QQ

berikut link Github kami: https://github.com/Indirarully/Kelompok-IOT/tree/main
