# Jarkom-Modul-1-E13-2023

SOAL

1. User melakukan berbagai aktivitas dengan menggunakan protokol FTP. Salah satunya adalah mengunggah suatu file.
   
   a.  Berapakah sequence number (raw) pada packet yang menunjukkan aktivitas tersebut?
      >>Cara pengerjaan:
      - Kata kunci pada soal tersebut adalah menggunggah suatu file
      - Mencari packet yang ada informasi mengenai pengunggahan suatu file 
      - Pada frame 147 didapatkan suatu informasi mengenai request pengunggahan file "Request: STOR c75-GrabThePhisher.zip"
      - Jika diklik 2 kali maka akan memberikan informasi lebih detail mengenai sequence number (raw) pada packet tersebut  
      - Sequence number (raw) = 258040667 

   b. Berapakah acknowledge number (raw) pada packet yang menunjukkan aktivitas tersebut? 
      >>Cara pengerjaan:
      - Didapatkan informasi mengenai acknowledge number (raw) dari frame sebelumnya, yaitu frame 147
      - Acknowledge number (raw) = 1044861039 

   c. Berapakah sequence number (raw) pada packet yang menunjukkan response dari aktivitas tersebut?
      >>Cara Pengerjaan:
      - Suatu packet yang melakukan request sesuatu kepada server, pasti memerlukan suatu response
      - Response yang berkaitan dengan GrabThePisher seperti request sebelumnya, terletak pada frame 149 dengan adanya informasi "Response: 150 Opening BINARY mode data connection for c75-GrabThePhisher.zip"
      - Maka sequence number (raw) pada packet yang menunjukkan response didapatkan, yaitu 1044861039 

   d. Berapakah acknowledge number (raw) pada packet yang menunjukkan response dari aktivitas tersebut?
      >>Cara pengerjaan:
      - Acknowledge number (raw) pada packet yang menunjukkan response didapatkan dari detail informasi pada frame sebelumnya
      - Acknowledge number (raw) = 258040696

      >>Screenshot pengerjaan:

      <img width="470" alt="soal1" src="https://github.com/Ulya321/Jarkom-Modul-1-E13-2023/blob/main/Images/soal1.png">
      <img width="470" alt="soal1" src="https://github.com/Ulya321/Jarkom-Modul-1-E13-2023/blob/main/Images/soal1_1.png">
   
2. Sebutkan web server yang digunakan pada portal praktikum Jaringan Komputer!
   >>Cara pengerjaan:
   - Karena soal mencari web server, pasti memiliki protocol http
   - Mencari di display filter dengan kata kunci "http"
   - Akan didapatkan dalam salah satu paket informasi mengenai web server yang berkaitan yaitu "Gunicorn"
   
      >>Screenshot pengerjaan:
   
3. Dapin sedang belajar analisis jaringan. Bantulah Dapin untuk mengerjakan soal berikut:
   a. Berapa banyak paket yang tercapture dengan IP source maupun destination address adalah 239.255.255.250 dengan port 3702?
      >>Cara pengerjaan:
      - Mencari di display filter dengan filter expression "ip.addr == 239.255.255.250 && port == 3702"
      - Akan didapatkan informasi mengenai banyaknya paket yang tercapture dengan ip adrress dan port seperti yang diminta yaitu sebanyak 21

   b. Protokol layer transport apa yang digunakan?
      >>Cara pengerjaan:
      - Dalam informasi paket menampilkan protokol apa yang dipakai dalam paket tersebut, yaitu UDP
     
     >>Screenshot pengerjaan:

      <img width="470" alt="soal1" src="https://github.com/Ulya321/Jarkom-Modul-1-E13-2023/blob/main/Images/soal3.png">
      
4. Berapa nilai checksum yang didapat dari header pada paket nomor 130?   
   >>Cara pengerjaan:
   - Mencari paket no 130 di display filter
   - Meng-klik 2 kali untuk mengetahui informasi lebih detail mengenai paket
   - Checksum didapatkan yaitu 0x18e5 

     Screenshot pengerjaan:

      <img width="470" alt="soal1" src="https://github.com/Ulya321/Jarkom-Modul-1-E13-2023/blob/main/Images/soal4.png">
      
5. Elshe menemukan suatu file packet capture yang menarik. Bantulah Elshe untuk menganalisis file packet capture tersebut.
   a. Berapa banyak packet yang berhasil di capture dari file pcap tersebut?
      >>Cara pengerjaan:
      - Setelah membuka file pcap, sudah terdapat informasi mengenai jumlah paket yaitu 60
   
   b. Port berapakah pada server yang digunakan untuk service SMTP?
      >>Cara pengerjaan:
      - Mengetikkan "smtp" pada display filter untuk mendapat kan service smtp
      - Pada frame 25, pada detail packet mengenai Tranmission Control Protocol didapatkan port yang dipakai adalah 25

   c. Dari semua alamat IP yang tercapture, IP berapakah yang merupakan public IP?
      >>Cara pengerjaan:
      - Terdapat 2 ip, yang merupakan smtp
      - Untuk mengetahui apakah keduanya merupakan public IP, kami menggunakan situs web "Checking ip address"
      - Didapatkan 1 ip address yang merupakan public ip yaitu 74.53.140.153.

      Screenshot pengerjaan:
         
      <img width="470" alt="soal1" src="https://github.com/Ulya321/Jarkom-Modul-1-E13-2023/blob/main/Images/soal5.png">\
      <img width="470" alt="soal1" src="https://github.com/Ulya321/Jarkom-Modul-1-E13-2023/blob/main/Images/soal5_1.png">\
      <img width="470" alt="soal1" src="https://github.com/Ulya321/Jarkom-Modul-1-E13-2023/blob/main/Images/soal5_2.png">\
      <img width="470" alt="soal1" src="https://github.com/Ulya321/Jarkom-Modul-1-E13-2023/blob/main/Images/soal5_3.png">\
      <img width="470" alt="soal1" src="https://github.com/Ulya321/Jarkom-Modul-1-E13-2023/blob/main/Images/soal5_4.png">\
      <img width="470" alt="soal1" src="https://github.com/Ulya321/Jarkom-Modul-1-E13-2023/blob/main/Images/soal5_5.png">
      
5. Seorang anak bernama Udin Berteman dengan SlameT yang merupakan seorang penggemar film detektif. sebagai teman yang baik, Ia selalu mengajak slamet untuk bermain valoranT bersama. suatu malam, terjadi sebuah hal yang tak terdUga. ketika udin mereka membuka game tersebut, laptop udin menunjukkan sebuah field text dan Sebuah kode Invalid bertuliskan "server SOURCE ADDRESS 7812 is invalid". ketika ketika ditelusuri di google, hasil pencarian hanya menampilkan a1 e5 u21. jiwa detektif slamet pun bergejolak. bantulah udin dan slamet untuk menemukan solusi kode error tersebut.
   >>Cara pengerjaan:
   Clue yang diberikan adalah sebagai berikut:
   - Clue 1: Sepertinya ada yang salah dengan penulisan tersebut secara KBBI. Ada sesuatu yang Besar di depan mata.
   - Clue 2: Jenis cipher merupakan substitusi a1z26 Cipher
   - Clue 3: Rentang Huruf yang digunakan Huruf A-R, 1-18 dengan Jawaban 6 Huruf.
   - Clue 4: SOURCE ADDRESS ADALAH KUNCI SEMUANYA.
   Dari clue-clue tersebut, kita lihat dulu pada packet 7812. Karena clue mengatakan bahwa source address adalah kunci dari semuanya maka kita lihat IP Source pada paket 7812. IP Sourcenya adalah 104.18.14.101. Selanjutnya untuk melakukan substitusi a1z26 cipher, kita hilangkan titik pada IP source terlebih dahulu menjadi 1041814101. Jika kita pecah menjadi angka yang kurang dari 26 maka menjadi 10 4 18 14 10 1. Dilakukanlah proses subtitusi dan mendapatkan hasil JDRNJA.

   Screenshot pengerjaan:
         
   <img width="470" alt="soal1" src="https://github.com/Ulya321/Jarkom-Modul-1-E13-2023/blob/main/Images/soal6.png">
   <img width="470" alt="soal1" src="https://github.com/Ulya321/Jarkom-Modul-1-E13-2023/blob/main/Images/soal6_1.png">
      
6. Berapa jumlah packet yang menuju IP 184.87.193.88?
   >>Cara pengerjaan:
   - Menggunakan kueri "ip.dst == 184.87.193.88" dan akan mendapatkan 6 paket yang terlihat

   Screenshot pengerjaan:
         
   <img width="470" alt="soal1" src="https://github.com/Ulya321/Jarkom-Modul-1-E13-2023/blob/main/Images/soal7.png">
      
7. Berikan kueri filter sehingga wireshark hanya mengambil semua protokol paket yang menuju port 80! (Jika terdapat lebih dari 1 port, maka urutkan sesuai dengan abjad)
   >>Cara pengerjaan:
   - Untuk mengambil semua protokol paket yang menuju port 80 maka kita dapat menggunakan kueri "tcp.dstport == 80 || udp.dstport == 80"
   
   Screenshot pengerjaan:
         
   <img width="470" alt="soal1" src="https://github.com/Ulya321/Jarkom-Modul-1-E13-2023/blob/main/Images/soal8.png">
   
8. Berikan kueri filter sehingga wireshark hanya mengambil paket yang berasal dari alamat 10.51.40.1 tetapi tidak menuju ke alamat 10.39.55.34!
   >>Cara pengerjaan:
   - Untuk mengambil paket yang berasal dari alamat 10.51.40.1 tetapi tidak menuju ke alamat 10.39.55.34 adalah menggunakan kueri "ip.src == 10.51.40.1 && ip.dst != 10.39.55.34"
    
   Screenshot pengerjaan:
         
   <img width="470" alt="soal1" src="https://github.com/Ulya321/Jarkom-Modul-1-E13-2023/blob/main/Images/soal9.png">
   
9. Sebutkan kredensial yang benar ketika user mencoba login menggunakan Telnet
   >>Cara pengerjaan:
   - Pada wireshark, kita filter dulu "Telnet" untuk memunculkan semua paket dengan protokol telnet
   - Setelah itu, kita cari dan perhatikan paket-paket yang terkait dengan proses login. Biasanya, login akan melibatkan beberapa paket yang mengirimkan kredensial (username dan password)
   - Pada paket 259 berisi sebuah data "Password:", hal ini mengindikasikan bahwa letak data password akan ada di paket setelah ini dan untuk username ada di sebelumnya
   - Pada paket 262 berisi sebuah data "kesayangannyak0k0", hal ini merupakan data password
   - Kemudian untuk username bisa dicari pada paket-paket yang ada di sebelum 259, tiap paket di sebelum paket 259 mengirimkan 1 huruf yang nantinya membentuk kata dhafin. Hal ini diperkuat juga dengan paket 81

   Screenshot pengerjaan:
         
   <img width="470" alt="soal1" src="https://github.com/Ulya321/Jarkom-Modul-1-E13-2023/blob/main/Images/soal10.png">
   <img width="470" alt="soal1" src="https://github.com/Ulya321/Jarkom-Modul-1-E13-2023/blob/main/Images/soal10_1.png">
   <img width="470" alt="soal1" src="https://github.com/Ulya321/Jarkom-Modul-1-E13-2023/blob/main/Images/soal10_2.png">

\
\
[CATATAN] Kendala/error yang dialami:
- VPN ITS yang tiba-tiba tidak dapat digunakan, "No Internet Connection" sehingga menghambat pengerjaan praktikum
- Belum selesai mengerjakan soal nomer 6 saat jadwal praktikum
