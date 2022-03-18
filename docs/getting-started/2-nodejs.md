---
sidebar_position: 2
---

# Node JS

import useBaseUrl from '@docusaurus/useBaseUrl';

:::caution
Bagian ini wajib dilakukan sebelum melanjutkan ke bagian selanjutnya
:::

**Node.js** adalah platform perangkat lunak yang dirancang oleh Ryan Lienhart Dahl. **Node.js** adalah runtime untuk lingkungan JavaScript di luar web browser yang dibangun di atas `v8 JavaScript Engine`. Node.js dapat dijalankan pada `Windows, Mac OS X, dan Linux`

## Kelebihan Node JS

1. Bekerja Dengan Konsep Non-blocking
   Node.js bekerja dengan konsep `non-blocking`. Misalnya begini, ada dua proses yang berjalan yaitu proses A dan proses B. Sayangnya proses A mengalami blocking karena suatu hal. Meskipun demikian, Anda masih tetap bisa menjalankan proses B jika proses ini tidak membutuhkan output dari proses A. Itulah yang disebut konsep non-blocking. Dengan demikian, akan terjadi efisiensi.

2. Cepat Dalam Mengeksekusi Kode
   **Kelebihan** lainnya yang dimiliki oleh Node.js adalah kemampuannya dalam mengeksekusi dengan cepat. Hal ini juga bisa terjadi berkat `engine V8 dari Google` yang digunakan untuk membuat Node.js

3. Single-threaded
   Node.js juga memiliki karakteristik `single-threade`d. Dengan karakter ini, program yang dibuat dengan Node.js akan mengalokasikan thread hanya pada proses yang sedang berlangsung sehingga kinerja program tersebut akan lebih ringan daripada program yang `multi-threaded`.

4. Open source
   Platform ini bersifat `open source`, artinya semua orang bisa melihat struktur kode dari program tersebut. Selain itu, Anda juga bisa berkontribusi untuk mengembangkan program tersebut agar bisa lebih baik. 

## Instalasi Node JS

1. Download Node.Js
   Download terlebih dahulu file installer VSCode melalui situs resminya [nodejs.org](https://nodejs.org/en/)

   <img alt="image2" src={useBaseUrl('img/docs/image-0-1.png')} height="500px"/>


2. Proses Instalasi
   - Double klik pada file installer nya atau klik kanan kemudian pilih Run as Administrator.
   - Jika muncul peringatan **Run as Administrator**, silahkan klik **Yes**.
   - Pilih “I accept the agreement” untuk menyetujui “License Agreement”, kemudian klik **Next**.
   - Untuk Select Destination Location bisa di biarkan saja jika lokasi instalasi tidak akan diubah. Klik **Next**
   - Lalu klik Install untuk memulai proses instalasi
   - Tunggu sampai proses instalasi selesai
   - Setelah selesai klik **Finish**