# Jarkom-Modul-1-E13-2023

SOAL

1. User melakukan berbagai aktivitas dengan menggunakan protokol FTP. Salah satunya adalah mengunggah suatu file.
   
a.  Berapakah sequence number (raw) pada packet yang menunjukkan aktivitas tersebut?

Cara pengerjaan:


   - Kata kunci pada soal tersebut adalah menggunggah suatu file
   
   - Mencari packet yang ada informasi mengenai pengunggahan suatu file
   
   - Pada frame 147 didapatkan suatu informasi mengenai request pengunggahan file "Request: STOR c75-GrabThePhisher.zip"
   
   - Jika diklik 2 kali maka akan memberikan informasi lebih detail mengenai sequence number (raw) pada packet tersebut

b. Berapakah acknowledge number (raw) pada packet yang menunjukkan aktivitas tersebut? 
Cara pengerjaan:
   >>Didapatkan informasi mengenai acknowledge number (raw) dari frame sebelumnya

c. Berapakah sequence number (raw) pada packet yang menunjukkan response dari aktivitas tersebut?
 Cara Pengerjaan:
   >>Suatu packet yang melakukan request sesuatu kepada server, pasti memerlukan suatu response
   >>Response yang berkaitan dengan GrabThePisher seperti request sebelumnya, terletak pada frame 149 dengan adanya informasi "Response: 150 Opening BINARY mode data            connection for c75-GrabThePhisher.zip"
   >>Maka sequence number (raw) pada packet yang menunjukkan response didapatkan

d. Berapakah acknowledge number (raw) pada packet yang menunjukkan response dari aktivitas tersebut?
Cara pengerjaan:
   >>acknowledge number (raw) pada packet yang menunjukkan response didapatkan dari detail informasi pada frame sebelumnya

2. Sebutkan web server yang digunakan pada portal praktikum Jaringan Komputer!
Cara pengerjaan:
   >>Karena soal mencari web server, pasti memiliki protocol http
   >>Mencari di display filter dengan kata kunci "http"
   >>AKan didapatkan dalam salah satu paket informasi mengenai web server yang berkaitan yaitu "Gunicorn"
   
3. Dapin sedang belajar analisis jaringan. Bantulah Dapin untuk mengerjakan soal berikut:
a. Berapa banyak paket yang tercapture dengan IP source maupun destination address adalah 239.255.255.250 dengan port 3702?
Cara pengerjaan:
   >>Mencari di display filter dengan filter expression "ip.addr == 239.255.255.250 && port == 3702"
   >>Akan didapatkan informasi mengenai banyaknya paket yang tercapture dengan ip adrress dan port seperti yang diminta

b. Protokol layer transport apa yang digunakan?
   >>Dalam informasi paket menampilkan protokol apa yang dipakai dalam paket tersebut.

4. Berapa nilai checksum yang didapat dari header pada paket nomor 130?
Cara pengerjaan:
   >>Mencari paket no 130 di display filter
   >>Meng-klik 2 kali untuk mengetahui informasi lebih detail mengenai paket
   >>Cheksum didapatkan
   
5. Elshe menemukan suatu file packet capture yang menarik. Bantulah Elshe untuk menganalisis file packet capture tersebut.
a. Berapa banyak packet yang berhasil di capture dari file pcap tersebut?
   >>Setelah membuka file pcap, sudah terdapat informasi mengenai jumlah paket
   
b. Port berapakah pada server yang digunakan untuk service SMTP?
   >>Mengetikkan "smtp" pada display filter untuk mendapat kan service smtp
   >>Pada frame 25, pada detail packet mengenai Tranmission Control Protocol didapatkan port yang dipakai adalah 25

c. Dari semua alamat IP yang tercapture, IP berapakah yang merupakan public IP?
   >>Terdapat 2 ip, yang merupakan smtp
   >>Untuk mengetahui apakah keduanya merupakan public IP, kami menggunakan situs web "Checking ip address"
   >>Didapatkan 1 ip address yang merupakan public ip.

8. Seorang anak bernama Udin Berteman dengan SlameT yang merupakan seorang penggemar film detektif. sebagai teman yang baik, Ia selalu mengajak slamet untuk bermain valoranT bersama. suatu malam, terjadi sebuah hal yang tak terdUga. ketika udin mereka membuka game tersebut, laptop udin menunjukkan sebuah field text dan Sebuah kode Invalid bertuliskan "server SOURCE ADDRESS 7812 is invalid". ketika ketika ditelusuri di google, hasil pencarian hanya menampilkan a1 e5 u21. jiwa detektif slamet pun bergejolak. bantulah udin dan slamet untuk menemukan solusi kode error tersebut.
   
9. Berapa jumlah packet yang menuju IP 184.87.193.88?
   
10. Berikan kueri filter sehingga wireshark hanya mengambil semua protokol paket yang menuju port 80! (Jika terdapat lebih dari 1 port, maka urutkan sesuai dengan abjad)
   
11. Berikan kueri filter sehingga wireshark hanya mengambil paket yang berasal dari alamat 10.51.40.1 tetapi tidak menuju ke alamat 10.39.55.34!
    
12. Sebutkan kredensial yang benar ketika user mencoba login menggunakan Telnet

