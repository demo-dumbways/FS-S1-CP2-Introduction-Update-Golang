---
sidebar_position: 4
---

# Heroku

import useBaseUrl from '@docusaurus/useBaseUrl';

<center>
<img src="https://www3.assets.heroku.com/assets/logo-purple-08fb38cebb99e3aac5202df018eb337c5be74d5214768c90a8198c97420e4201.svg" style={{backgroundColor: 'white', padding: 10, borderRadius: 10, width: '50%'}} />
</center>

<div style={{marginTop: 50}}>
<b>Heroku</b> adalah sebuah cloud platform yang menjalankan bahasa pemrograman tertentu, Heroku mendukung bahasa pemrograman seperti Ruby, Node.js, Python, Java, PHP, dan lain-lain.
</div>

<div style={{marginTop: 10}}>
Heroku termasuk ke dalam kriteria Platform As A Service (PaaS), sehingga bagi anda yang ingin melakukan deploy aplikasi ke heroku cukup hanya dengan melakukan konfigurasi aplikasi yang ingin di deploy dan menyediakan platform yang memungkinkan pelanggan untuk mengembangkan, menjalankan, dan mengelola aplikasi tanpa kompleksitas membangun dan memelihara infrastruktur yang biasanya terkait dengan pengembangan dan peluncuran aplikasi.
</div>

<br />

Visit: [heroku](https://www.heroku.com)

## Deploy Express App to Heroku

- Silakan buat akun & login
- Pada halaman dashboard, buat aplikasi baru dengan klik `new` pada tombol atas kanan dan pilih `Create new app`
   <center>
      <img src={useBaseUrl('img/docs/heroku-2.png')} style={{ width: '60%'}} />
   </center>
- Ketik nama aplikasi dan klik `Create app`
   <center>
      <img src={useBaseUrl('img/docs/heroku-3.png')} style={{ width: '80%'}} />
   </center>

- Pada bagian `Deploy`, pilih `Deployment method` -> `Github`
   <center>
      <img src={useBaseUrl('img/docs/heroku-5.png')} style={{ width: '80%'}} />
   </center>
- Cari repository project Anda dan klik `Connect`
   <center>
      <img src={useBaseUrl('img/docs/heroku-6.png')} style={{ width: '80%'}} />
   </center>
- Pastikan `Automatic deploys` sudah `Enable` dan klik `Deploy Branch`
   <center>
      <img src={useBaseUrl('img/docs/heroku-7.png')} style={{ width: '80%'}} />
   </center>
- Jika terdapat tulisan `Your app was successfully deployed` artinya Anda berhasil melakukan Deploy
    <center>
      <img src={useBaseUrl('img/docs/heroku-8.png')} style={{ width: '80%'}} />
   </center>
- Klik `Open App` untuk membuka app yang telah terdeploy
   <center>
      <img src={useBaseUrl('img/docs/heroku-9.png')} style={{ width: '80%'}} />
   </center>

## Database on Heroku

- Pada bagian `Resources`, cari `Heroku Postgres` pada `Add-ons`
   <center>
      <img src={useBaseUrl('img/docs/heroku-db-1.png')} style={{ width: '80%'}} />
   </center>

- Pilih plan name `Hobby Dev - Free` dan klik tombol `Submit Order Form`
    <center>
      <img src={useBaseUrl('img/docs/heroku-db-2.png')} style={{ width: '80%'}} />
   </center>
- Anda telah berhasil membuat database, selanjutnya klik `Heroku Postgres` untuk melihat `Database Credentials` yang akan digunakan untuk koneksi ke database
   <center>
      <img src={useBaseUrl('img/docs/heroku-db-3.png')} style={{ width: '80%'}} />
   </center>
   <center>
      <img src={useBaseUrl('img/docs/heroku-db-4.png')} style={{ width: '80%'}} />
   </center>
- Buka aplikasi `PgAdmin` dan `create server`
   <center>
      <img src={useBaseUrl('img/docs/heroku-db-5.png')} style={{ width: '80%'}} />
   </center>
- Isi konfigurasi create server pada bagian `General`, `Connection`, dan `Advanced`
    <center>
      <img src={useBaseUrl('img/docs/heroku-db-6.png')} style={{ width: '60%'}} />
   </center>
    <center>
      <img src={useBaseUrl('img/docs/heroku-db-7.png')} style={{ width: '60%'}} />
   </center>
    <center>
      <img src={useBaseUrl('img/docs/heroku-db-8.png')} style={{ width: '60%'}} />
   </center>
- Aplikasi `PgAdmin` telah berhasil koneksi ke `database heroku`. Anda dapat membuat tabel yang disesuaikan dengan tabel pada `local database` Anda.
   <center>
      <img src={useBaseUrl('img/docs/heroku-db-9.png')} style={{ width: '40%'}} />
   </center>
