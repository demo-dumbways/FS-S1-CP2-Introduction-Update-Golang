---
sidebar_position: 3
---

# PostgreSQL

:::info
Bagian ini boleh diabaikan terlebih dahulu, karena pada beberapa bagian selanjutnya akan diarahkan kembali ke bagian ini
:::

import useBaseUrl from '@docusaurus/useBaseUrl';

**PostgreSQL** atau **(Post-gress-SQL)** adalah sebuah relational database manajemen system  (RDBMS) yang di kembangkan oleh tim relawan yang ada di seluruh dunia yang bersifat open source. PostgreSQL tidak di kontrol oleh perusahaan atau badan swasta lainnya sehingga source code (kode sumber) yang tersedia bisa di dapatkan secara gratis.

PostgreSQL dapat berjalan di semua sistem operasi termasuk (Linux, UNIX (AIX, BSD, HP-UX, SGI IRIX, Mac OS X, Solaris, Tru64), and Windows. PostgreSQL mendukung teks, gambar, suara, dan video, dan termasuk antarmuka pemrograman untuk C / C ++, Java, Perl, Python, Ruby, Tcl dan Open Database Connectivity (ODBC).

PostgreSQL mendukung sebagian besar dari standar SQL dan menawarkan banyak fitur modern termasuk dibawah ini:

- Complex SQL queries
- SQL Sub-selects
- Foreign keys
- Trigger
- Views
- Transactions
- Multiversion concurrency control (MVCC)
- Streaming Replication (as of 9.0)
- Hot Standby (as of 9.0)

## Instalasi PostgreSQL

1. Download Node.Js
   Download terlebih dahulu file installer `PostgreSQL` melalui situs resminya [postgresql.org](https://www.postgresql.org/download/)

   <img alt="image2" src={useBaseUrl('img/docs/image-0-2.png')} width="100%"/>

2. Proses Instalasi
   - Double klik pada file installer nya atau klik kanan kemudian pilih Run as Administrator.
   - Jika muncul peringatan **Run as Administrator**, silahkan klik **Yes**.
   - Pilih “I accept the agreement” untuk menyetujui “License Agreement”, kemudian klik **Next**.
   - Pilih prefered language
   - Untuk Select Destination Location, bisa di biarkan saja jika lokasi instalasi tidak akan diubah. Klik **Next**
   - Isikan port yang akan digunakan untuk menjalankan postgresql, bisa di biarkan saja jika lokasi instalasi tidak akan diubah. Klik **Next**
   - Isikan path directory untuk penyimpanan file database, bisa di biarkan saja jika lokasi instalasi tidak akan diubah. Klik **Next**
   - Buat password untuk user PostgreSQL
   - Lalu klik Install untuk memulai proses instalasi
   - Tunggu sampai proses instalasi selesai
   - Setelah selesai klik **Finish**