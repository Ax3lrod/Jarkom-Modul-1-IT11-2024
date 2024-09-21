# Jarkom-Modul-1-IT11-2024

IT 11
Aryasatya Alaauddin 5027231082
Almendo Jekson Darwin Naftali Kambu 5027221073

## Advance Sanity Check

![image](https://github.com/user-attachments/assets/c0356468-f9de-401e-b0ec-61be37df07ba)

Soal memberikan file sanity.pcapng dan command ncat 10.15.42.60 44000. Dari ncat yang dijalankan muncul pertanyaan: 
```
Apa username pengirim?
Format: username
```
Jawabannya dapat ditemukan di file .pcapng dengan menggunakan wireshark.
![image](https://github.com/user-attachments/assets/3b1bf520-7d06-4996-ba62-f47b7230a931)
Jawabannya adalah: JaneD03

Pertanyaan berikutnya adalah:
Apa nama file yang dikirim?
Format: filename.extension

Jawabannya dapat ditemukan di file .pcapng dengan menggunakan wireshark.
![image](https://github.com/user-attachments/assets/fcfeed73-902b-437e-b7e1-a094f16cfea6)

Pertanyaan berikutnya:
Ikuti petunjuk untuk mendapatkan pesan rahasia
Format: string

Petunjuk yang saya dapatkan mengarahkan saya ke canva peraturan praktikum jarkom.
![image](https://github.com/user-attachments/assets/127e5302-3e5d-4b98-a476-0468f4195ca6)

String tersebut saya decrypt menggunakan base64 dan mendapatkan string penword. Menginput string tersebut memberikan flagnya.
Ikuti petunjuk untuk mendapatkan pesan rahasia
```
Format: string
> penword
Benar! Ini flag-mu: JarkomIT{8uK4n_S4n1ty_b1a5A_WdGytApziiDNfEwyy1xtbWWU2Su51qz4XWMS5QSa5BWFO4cexyRkcIKK}
```

## EZ

![image](https://github.com/user-attachments/assets/8e7b2940-5647-4627-a8e9-2064597d52b0)

chall memberikan file .pcapng dan port ncat.
ncat memberikan pertanyaan:
```
===== EZ =====
Note: You can exit anytime by typing 'exit'

Temukan jawaban dari log tersebut
Format: string ex. kata kata
```

dengan membuka file .pcapng di wireshark saya menemukan
![image](https://github.com/user-attachments/assets/537e7ef3-39e7-4230-a09b-d076e466375e)

dengan memberikan input ```jawabannya jawaban``` saya mendapatkan pertanyaan berikutnya:
```
Port berapa yang digunakan service tersebut
Format: xxxx: ex. 443
```
dengan memeriksa metadata package saya menemukan portnya
![image](https://github.com/user-attachments/assets/5487f902-81ef-4fa0-8e02-b27b7ff61390)

setelah memasukkan input 1234 saya mendapatkan flagnya:

```
Port berapa yang digunakan service tersebut
Format: xxxx: ex. 443
> 1234
Benar! Ini flag-mu: JarkomIT{BiAr_aman_Pake_sSh_IoKgV4MjC31VD34DsBnBMr7ub3znaXU69C4RHT50mwYc9Zo5vTTaEZ}
```

## Pegawai Negeri Sebelah

![image](https://github.com/user-attachments/assets/4aa30877-3bd9-4fd6-a09e-b700f1fdb676)

Seperti chall lainnya saya diberikan file pcapng dan port ncat. 
membuka port ncatnya memberikan saya pertanyaan:

```
Siapa yang memiliki password nNnM%coQuF?
Format: String
```

setelah mengeksplor file .pcapng nya menggunakan wireshark saya menemukan database akun pns.
![image](https://github.com/user-attachments/assets/d7d8cb5a-ccd7-4ab9-a7bf-16a2bf6d4119)

disana saya menemukan pemilik password yang diberikan yaitu Vero Tampubolon.
Kemudian saya diberikan 3 pertanyaan lain yang dimana semua jawabannya saya temukan di database yang sama. Menjawab semua pertanyaannya memberikan saya flag.

```
=====  Pegawai Negeri Sebelah =====
Note: You can exit anytime by typing 'exit'

Siapa yang memiliki password nNnM%coQuF?
Format: String
> Vero Tampubolon
Apa jabatan dari Taufan Kuswandari?
Format: String
> Analis Kebijakan
Siapa yang paling awal di list?
Format: String
> Cici Mustofa
Apa password paling akhir dari list?
Format: String
> RyxaJPv^yF
Benar! Ini flag-mu: JarkomIT{Tum8eN_p45SnYa_Ku4t_B1aS4Nya_1EGvtVltmagyAhMBWa2EHaFGqL3wSEeWrf6Pzy23l3QHQFJcFhBSM4h}
```

## FTP Login

![image](https://github.com/user-attachments/assets/5beab75f-6c12-4285-84d1-74dece1bb4ce)

membuka port ncat memberikan saya pertanyaan:

```
===== FTP Login =====
Note: You can exit anytime by typing 'exit'

Apa username yang berhasil digunakan untuk FTP login?
Format: username
```

setelah mengeksplor file pcapng yang diberikan menggunakan wireshark saya menemukan username dan password yang terakhir digunakan hingga  berhasil login:
![image](https://github.com/user-attachments/assets/a223f2cd-a8f0-42be-b75e-9cbe676b4567)

dengan menginput sn34ky saya mendapatkan pertanyaan berikutnya:
```
Apa password yang berhasil digunakan untuk FTP login?
Format: string
```

berdasarkan temuan saya tadi saya juga mendapatkan password yang digunakan jadi saya langsung menginputkannya. Setelah melakukan itu saya mendaptakan flagnya:
```
===== FTP Login =====
Note: You can exit anytime by typing 'exit'

Apa username yang berhasil digunakan untuk FTP login?
Format: username
> sn34ky
Apa password yang berhasil digunakan untuk FTP login?
Format: string
> sup3rsn1ff3r
Benar! Ini flag-mu: JarkomIT{n0t_s0_s3cur3_ftp_ldIbqSfFj52A0fVMXvxtgvVkVL0Gzw7SieMZUto1SlUkFL216ww1G1N}
```

## Gajah Terbang (Server Recon)

![image](https://github.com/user-attachments/assets/de0b1626-0965-4f50-b614-8f19ebb533a2)

Membuka port ncat yang diberikan saya diberikan pertanyaan:
```
===== Gajah Terbang (Server Recon) =====
Note: You can exit anytime by typing 'exit'

Apa DBMS yang digunakan pada server tersebut?
Format: string ex. MonggoDB
```

Setelah membuka file pcapng nya menggunakan wireshark dan memeriksa data salah satu paket saya menemukan bahwa dbms yang digunakan adalah PostgreSQL:
![image](https://github.com/user-attachments/assets/178ff1ee-647b-495a-a2b5-369299aeeee9)

Pertanyaan berikutnya adalah:
```
Apa DBMS yang digunakan pada server tersebut?
Format: string ex. MonggoDB
> PostgreSQL
Di port berapa DBMS server tersebut berjalan?
Format: xxxx ex. 443
```

Setelah memeriksa kembali file pcapngnya di wireshark saya menemukan bahwa port yang digunakan dbms adalah 6969

![image](https://github.com/user-attachments/assets/6dbce010-fcc6-421a-a5ee-72e8cb239f0d)

setelah menginput jawaban tersebut saya mendapatkan pertanyaan berikutnya:
```
Di port berapa DBMS server tersebut berjalan?
Format: xxxx ex. 443
> 6969
OS apa yang digunakan untuk server tersebut?
Format: string ex. linux
```

Saya menemukan informasi os di salah satu paket:
![image](https://github.com/user-attachments/assets/669fec48-73ed-4e92-92c1-c930d84d7029)

menginput Debian saya mendapatkan pertanyaan berikutnya:
```
Apa credentials username DBMS valid yang digunakan?
Format: string
```

dari follow paket yang sama saya menemukan jawabannya:
![image](https://github.com/user-attachments/assets/4ceccc5b-f3c3-4aa3-a22b-b783203cea38)

Pertanyaan berikutnya:
```
Apa nama database yang digunakan?
Format: string
```

jawabannya juga saya dapatkan dari tempat yang sama yaitu sigmaskibidigyatrizzzz

![image](https://github.com/user-attachments/assets/7e5ff905-3d75-4439-b656-f53062657d29)

pertanyaan berikutnya:
```
Ada berapa banyak users dalam database tersebut?
Format: number
```

dari tempat yang sama saya menghitung semua user dan mendapatkan jumlah 4
![image](https://github.com/user-attachments/assets/aaa26bb0-b398-46f5-94bc-08eae60fd25b)

pertanyaan berikutnya:
```
Apa email yang digunakan oleh admin?
Format: email@gmail.com
```

dari tempat yang sama saya menemukan bahwa jawabannya adalah jojohermawan@gmail.com:

![image](https://github.com/user-attachments/assets/3da54e5c-f0d1-4c2c-8393-403d5f710458)

dari sana saya juga menemukan jawaban untuk pertanyaan berikutnya yaitu password untuk akun Jojo Hermawan yang harus didecrypt terlebih dahulu menggunakan MD5
![image](https://github.com/user-attachments/assets/18a01c4a-56ae-4ef0-b2d4-7effba61c0e4)

. Menjawab pertanyaan itu memberikan saya flagnya:
```
Apa email yang digunakan oleh admin?
Format: email@gmail.com
> jojohermawan@gmail.com
Apa password yang digunakan oleh admin?
Format: string
> admin1234
Benar! Ini flag-mu: JarkomIT{Gy4tT_M5g_4U_9DaFiMOmVtjHqnS0LlKQUbR6S5k1EKEYYYsYjdblQ1SbEUhOhUjjVBiD1}
```

## Gajah Terbang (Attacker Recon)
![image](https://github.com/user-attachments/assets/90e3d44f-4996-434f-bb5f-63353755fb8b)

pertanyaan1:
```
===== Gajah Terbang (Attacker Recon) =====
Note: You can exit anytime by typing 'exit'

Akun apa yang dimiliki oleh penyerang dalam database tersebut, berikan emailnya!
Format: user@gmail.com
```

Jawaban:

Chall ini masih menggunakan pcapng chall gajah terbang sebelumnya.
Dengan mencoba coba semua email yang ada di database saya menemukan bahwa jawabannya adalah kuntoajiisrillll@gmail.com

pertanyaan2:
```
Akun apa yang dimiliki oleh penyerang dalam database tersebut, berikan emailnya!
Format: user@gmail.com
> kuntoajiisrillll@gmail.com
Apa password yang digunakan oleh penyerang?
Format: string
```

password saya temukan di tempat yang sama dan harus didecrypt terlebih dahulu menggunakan md5:
![image](https://github.com/user-attachments/assets/05d119ee-5ff9-4c6c-ae4e-5b540a6c8c2e)
![image](https://github.com/user-attachments/assets/30a1f54a-0c8b-4898-ab9f-47c825498db0)

pertanyaan3:
```
Pada tanggal berapa akun penyerang diban?
Format:  YYYY-MM-DD
ex. 1945-08-17
```

Jawabannya saya temukan masih di tempat yang sama:

![image](https://github.com/user-attachments/assets/2a9c2063-c947-40d9-8746-f8492db913a6)

Pertanyaan 4:
```
Table apa saja yang dimodifikasi oleh penyerang?
Format: string dan string
> users dan banned_users
```

Berdasarkan semua tabel yang ada di database saya menemukan bahwa tabel yang dimodifikasi adalah users dan banned_users:
![image](https://github.com/user-attachments/assets/4c7788fc-0ade-44e8-8f30-c3f5415b737c)

Pertanyaan 5:

```
Barang apa saja yang telah dibeli oleh penyerang?
Format: string dan string
```

dengan mencoba coba semua kombinasi pasangan dari semua barang belanjaan yang tersedia saya menemukan bahwa jawabannya adalah rokok dan es krim

Pertanyaan 6:

```
Barang apa saja yang telah dibeli oleh penyerang?
Format: string dan string
> rokok dan es krim
Berapa total transaksi dari barang yang dibeli oleh penyerang?
Format: number
```

dengan menjumlahkan kedua harga dari rokok dan eskrim saya mendapatkan jawaban dan flagnya:

```
Barang apa saja yang telah dibeli oleh penyerang?
Format: string dan string
> rokok dan es krim
Berapa total transaksi dari barang yang dibeli oleh penyerang?
Format: number
> 24500
Benar! Ini flag-mu: JarkomIT{G4jaH_K0k_t3RbaNG_vIHSZLsDffacq38To2aa0td1fYntDCTJEuTWxXjkgF62BTsDfJfV3Kt5}
```

## Rizzset

![image](https://github.com/user-attachments/assets/ffafd565-4c50-42ec-95f7-5ded346a700d)

Pertanyaan1:
```
Apa nama domain dari dns query pada log?
Format: www.domain.com
> www.its.ac.id
```

Jawaban saya dapatkan dari file .pcapng yang diberikan:

![image](https://github.com/user-attachments/assets/cc31c50e-72c5-4cb5-a557-1246245cd19b)

Pertanyaan 2:
```
berapa IP dari domain tersebut?
Format: xxx.xxx.xxx.xxx
> 103.94.189.5
```

Jawabannya saya temukan di file .pcapng yang diberikan:
![image](https://github.com/user-attachments/assets/d16eac28-f413-4a8a-a09c-fdee9dbe60f8)

Pertanyaan 3:
```
Tuliskan JARM Fingerprint yang dihasilkan dari domain tersebut
Format: string
```

Untuk menemukan jawabannya saya menggunakan website https://jarm.online/ dan saya berikan domain website its:

![image](https://github.com/user-attachments/assets/25dda844-4cba-4f0f-bd7f-db34660e8b80)

Menginputkan hasilnya memberikan saya flagnya:
```
Tuliskan JARM Fingerprint yang dihasilkan dari domain tersebut
Format: string
ex. abcdef0123456789abcdef0123456789abcdef0123456789abcdef01234567
> 2ad2ad16d2ad2ad22c2ad2ad2ad2ad74aaecca9f9c4a3303863dfee62b241e
Benar! Ini flag-mu: JarkomIT{Dn5_C0rR34t10n_pXFijqYnQsoEkYSILjukdhW4cr1zZFxHtExj206S9mwDkxRci1579z1T5}
```

## Corporate Breach

![image](https://github.com/user-attachments/assets/cbcb3efa-59d0-47e0-8aa1-a7567762717c)

Pertanyaan1:
```
===== Corporate Breach =====
Note: You can exit anytime by typing 'exit'

Siapa nama attacker?
Format: string
```

saya menemukan jawabannya dengan memeriksa salah satu paket http di awal traffic dan menemukan bahwa attacker memperkenalkan dirinya:

![image](https://github.com/user-attachments/assets/a979ca6c-2130-48ec-8a6c-1af7decd8be1)

Pertanyaan2:
```
Apa email yang digunakan untuk login?
Format: email@gmail.com
```

Untuk mendapatkan jawaban ini saya pertama perlu mencari email dan password mana yang benar. Setelah memeriksa seluruh login request saya menemukan :
![image](https://github.com/user-attachments/assets/88def4e2-6b14-4a39-8200-f4d2f086d58c)

dimana hasil login menggunakan jarkomsupport@gmail.com mendapatkan respon yang berbeda (tidak ada login failed)

Pertanyaan3:
```
Apa password yang digunakan untuk login?
Format: string
> j4rk0mg4c0rbg
```
Dari packet yang sama saya juga menemukan passwordnya dan setelah menginputkannya saya mendapatkan flag:
```
Apa password yang digunakan untuk login?
Format: string
> j4rk0mg4c0rbg
Benar! Ini flag-mu: JarkomIT{supp0rt_k0k_l3m4h_bg_UDvIW6DQ0jTYHLw0YHEIrOWVKG6n6apHaGeaOCvLrDPxIHqHvzovG6}
```

## Malicious Code

![image](https://github.com/user-attachments/assets/c3f864ae-6e1b-4500-9749-72e3a88d7121)

Pertanyaan1:
```
===== Malicious Code =====
Note: You can exit anytime by typing 'exit'

Berapa total attempt attacker melakukan dir listing?
Format: number
```

Saya menemukan jawbannya dengan melakukan filter http.request.method == "GET" dan melihat berapa banyak file yang ditampilkan:

![image](https://github.com/user-attachments/assets/f7b7a1e6-a2f8-4185-96ee-c0653e9b23ca)

Pertanyaan2:
```
Apa endpoint yang berhasil attacker dapatkan untuk login page?
Format: /endpoint/path.php
```

Dengan memeriksa file pcapngnya dengan wireshark saya menemukan jawabannya adalah /index.php:
![image](https://github.com/user-attachments/assets/c3305ce8-ca4b-403c-936c-92b59540db5e)

Pertanyaan3:
```
Pada attempt ke berapa attacker menemukan email dan password yang benar?
Format: number
```

Untuk mendapatkan jawaban ini saya pertama perlu mencari email dan password mana yang benar. Setelah memeriksa seluruh login request saya menemukan :
![image](https://github.com/user-attachments/assets/88def4e2-6b14-4a39-8200-f4d2f086d58c)

dimana hasil login menggunakan jarkomsupport@gmail.com mendapatkan respon yang berbeda (tidak ada login failed) maka saya menghitung jumlah attempt dari sana dan menemukan jumlah 153:

Pada attempt ke berapa attacker menemukan email dan password yang benar?
Format: number
> 153

Pertanyaan 4:
```
Apa jawaban dari pertanyaan sang attacker?
Format: string
```

Setelah memeriksa kembali file, saya menemukan bahwa clue terakhir yang diberikan attacker sebelum pergi adalah:

9711297321199711411097321029711811111410511632112101109981179711632991049710810810111010310163324010410511011658321151191019711610111441

saya mencoba untuk merubah bentuknya dari descimall ke ascii menggunakan https://onlinetools.com/ascii/convert-decimal-to-ascii:

![image](https://github.com/user-attachments/assets/decf9c77-8912-408e-95e0-38097ace1a2b)

jujur mencoba coba semua warna dan menemukan bahwa jawabannya adalah merah dan mendapatkan flagnya:

```
Apa jawaban dari pertanyaan sang attacker?
Format: string
> merah
Benar! Ini flag-mu: JarkomIT{s3cr3t_m3ss4ge_fr0m_4uth0r_1awVLvEoPCj7G9X9ckNjIbIDRC0by3RlD25LQqK3tXMCuEAoYKQlL0R}
```

## Surprise

![image](https://github.com/user-attachments/assets/83292910-75b9-499f-9dfe-9a5e3a8ca7fd)

Pertanyaan1:
```
Apa service yang digunakan pada FTP server?
Format: service ver
ex. proFTPd 1.1.0
```

Setelah memfilter file FTP dan melakukan follow saya menemukan jawabannya:

![image](https://github.com/user-attachments/assets/a4bdd376-7f66-4863-9711-4b4f3bae0819)

Pertanyaan2:
```
Apa nama file yang dikirim oleh attacker?
Format: filename.extension
```

Masih menggunakan filter FTP saya menemukan nama file yang dikirim oleh attacker:
![image](https://github.com/user-attachments/assets/37165c26-5ead-4ea3-9d35-69bb97572438)

Pertanyaan3:
```
Apa pesan rahasia yang ditinggalkan oleh attacker?
Format: string ex. h4lo wor1d
```

Memfilter menggunakan FTP-DATA saya menemukan isi g0tcha.cpp :
```
#include <iostream>
#include <string>
#include <vector>
using namespace std;

string generateString() {
    auto tochip = [](int num) -> string {
        string chipStr;
        if (num < 0 || num > 255) return "";
        char buffer[3];
        snprintf(buffer, sizeof(buffer), "%02x", num);
        chipStr = buffer;
        return chipStr;
    };

    vector<int> chipParts = {103, 48, 116, 99, 104, 117, 32, 110, 48, 119, 32, 108, 49, 116, 116, 108, 51, 32, 109, 48, 117, 115, 51};

    string result;
    for (int part : chipParts) {
        result += static_cast<char>(part);
    }

    return result;
}

int main() {
    string result = generateString();

    cout << result << endl;

    return 0;
}
```

Program ini saya coba jalankan di https://www.programiz.com/cpp-programming/online-compiler/ dan mendapatkan string g0tchu n0w l1ttl3 m0us3

![image](https://github.com/user-attachments/assets/a5895577-6b41-4d39-8a0a-31376a2b637f)

Menginputkan string tersebut memberikan saya flagnya:
```
Apa pesan rahasia yang ditinggalkan oleh attacker?
Format: string ex. h4lo wor1d
> g0tchu n0w l1ttl3 m0us3
Benar! Ini flag-mu: JarkomIT{l1ttl3_m0us3_1n_th3_h0us3_gggrQxvaVoZGLvLl9CM4dAIEtG0uNS6meuS13AP3PqEKpVnv4eeQTCHU}
```

## Illegal Breakthrough
![image](https://github.com/user-attachments/assets/1c06ad8b-85c8-473f-a4e3-cf3178719076)

Pertanyaan 1:
```
===== Illegal Breakthrough =====
Note: You can exit anytime by typing 'exit'

Apa IP address dari korban?
Format: xxx.xxx.xxx.xxx
```

Setelah memeriksa file pcapng saya menemukan ip address destination dari setiap brute force attemp adalah 172.21.88.207
![image](https://github.com/user-attachments/assets/de341a88-45b7-4f30-85f6-ed4ecd2e5037)

Pertanyaan 2:
```
Apa port yang digunakan sebagai webserver?
Format: xxxx: ex. 443
```

![image](https://github.com/user-attachments/assets/23d93ac4-e2a1-443d-ba57-d774edb3d074)

Dari paket yang sama saya menemukan bahwa port dari webserver korban adalah 1917

Pertanyaan 3:
```
Dimana endpoint yang terdapat login?
Format: /endpoint/path.php
```
Karena setiap percobaan bruteforce dilakukan di /ww1.php maka saya coba itu sebaga input dan ternyata benar jawabannya:

![image](https://github.com/user-attachments/assets/edc03e72-a67f-40d4-a3e6-5f9fff189ce2)

Pertanyaan 4:
```
Tools apa yang digunakan oleh attacker?
Format: toolsname-version ex. hydra-v9.0-dev
```

Setelah saya melakukan follow pada packet percobaan bruteforce, saya menemukan:

![image](https://github.com/user-attachments/assets/eb1dba61-66b1-414e-8fac-53844b43a920)

Setelah memeriksa di internet saya menemukan bahwa nama lain dari Fuzz Faster U Fool v2.1.0-dev adalah ffuf-v2.1.0-dev

Pertanyaan 5:
```
Apa kredensial yang berhasil digunakan oleh attacker untuk login?
Format: username:password
```

Di attempt terakhir sebelum berhasil login, attacker memasukkan kredensial berikut:
![image](https://github.com/user-attachments/assets/f2ac341a-f853-4976-8439-d7fe5a49d6db)

memberikan input tersebut sesuai format memberikan saya flagnya:
```
Apa kredensial yang berhasil digunakan oleh attacker untuk login?
Format: username:password
> Redbaron:fly1ng4c3
Benar! Ini flag-mu: JarkomIT{d34th_fr0m_th3_sky_wo0eOYeGT17Dab3i2VWhkLtQaH1R1MDOx8eWW5pCSSOzLTxXl4EbWW1}
```

# Packets Barrage
![image](https://github.com/user-attachments/assets/325de92a-e01f-4ec6-a2ba-be8938f6091b)

Chall menggunakan file pcapng yang sama dengan challenge Illegal Breakthrough
Menjalankan Ncat yang diberikan saya mendapatkan pertanyaan

Pertanyaan 1:
```
Apa IP address dari attacker?
Format: xxx.xxx.xxx.xxx
```
Dengan memeriksa file pcapng yang diberikan menggunakan wireshark saya melihat request http POST ke ww1.php dimana attacker berusaha melakukan login dengan bruteforce. Dari setiap paket tersebut, source IP addressnya adalah 172.21.80.1
![image](https://github.com/user-attachments/assets/1b3ad50a-c3b1-43b7-948d-013a2568286c)

Menginput IP tersebut, saya mendapatkan pertanyaan berikutnya

Pertanyaan 2:
```
Berapa total attempt dari bruteforce attacker?
Format: number
```
Langkah pertama yang saya lakukan adalah melakukan filter untuk melihat semua paket http protocol yang melakukan request POST. Dari sana saya mendapatkan 1918 file. Namun ketika menginputkan 1918 itu bukan jawaban yang benar, tetapi ketika saya mengurangi 1 kepada jumlahnya menjadi 1917 saya mendapatkan jawaban yang benar.
![image](https://github.com/user-attachments/assets/2282e1d7-5ad9-41f1-9b76-5bb926c2345a)

Pertanyaan 3:
```
Apa nama file yang didownload oleh attacker setelah berhasil login?
Format: filename.extension
```
Langkah pertama saya adalah melihat apa yang dilakukan attacker setelah berhasil login. Disana saya menemukan bahwa attacker melakukan http protocol dengan request GET untuk mengunduh sebuah file. Melakukan follow pada paket tersebut saya menemukan bahwa paket yang diunduh adalah Albatros.txt.

![image](https://github.com/user-attachments/assets/70ab65e4-d768-4a54-9d1e-0a790bb503a7)

Pertanyaan 4:
```
Apa isi dari file yang disisipkan oleh attacker?
Format: string ex. sine sole nihil sum
```

Untuk jawaban dari pertanyaan ini saya temukan di tempat yang sama dengan jawaban sebelumnya. Isi dari filenya adalah Der "Rote Kampfflieger".

![image](https://github.com/user-attachments/assets/7444ddfe-3076-495d-8f96-9acec038ec66)

Menjawab pertanyaan tersebut memberikan saya flagnya:
```
Apa isi dari file yang disisipkan oleh attacker?
Format: string ex. sine sole nihil sum
> Der Rote Kampfflieger
Benar! Ini flag-mu: JarkomIT{th3_fly1ng_c1rcus_0f_w4r_bk0OU68kOzKM02fZGQfuQAdDK5Stjl7pKLukrtDexxEwPg2cKxddRACE}
```


