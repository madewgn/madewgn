---
comments: true
date: "2021-07-12T00:00:00Z"
subtitle: Cara membuat Bot Radio di Telegram dengan heroku
tags:
- Bot
title: Cara membuat Bot Radio di Telegram
---

# Pemutar Radio Telegram V3


Bot Telegram untuk Memutar Radio/Musik/YouTube Live di Saluran atau Obrolan Suara Grup.

Ini juga merupakan kode sumber bot yang digunakan untuk bermain
Radio di [AsmSafone](https://t.me/AsmSafone) Saluran & Musik di Grup [SafoTheBot](https://t.me/safothebot).

## Fitur spesial

- Daftar putar, antrean, aliran radio 24x7
- Mendukung streaming langsung dari youtube
- Mulai Radio setelah jika tidak ada lagu dalam daftar putar
- Pemutaran otomatis bahkan jika heroku dimulai ulang
- Tampilkan posisi pemutaran audio saat ini
- Kontrol dengan tombol dan perintah
- Unduh lagu dari youtube sebagai audio
- Secara otomatis mengunduh audio untuk dua trek pertama dalam daftar putar untuk memastikan pemutaran yang lancar

## Terapkan ke Heroku (Cara Mudah)



[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/AsmSafone/RadioPlayer/tree/V3.0) 
CATATAN: Pastikan Anda Telah Memulai Obrolan Suara Di Saluran/Grup Anda Sebelum Menyebarkan!

## Heroku Vars:
1. `API_ID` : Dapatkan Dari my.telegram.org
2. `API_HASH` : Dapatkan Dari my.telegram.org
3. `BOT_TOKEN` : Dapatkan Dari @Botfather
4. `SESSION_STRING` : Hasilkan Dari [@genStr robot](http://t.me/genStr_robot).
5. `CHAT` : ID Channel/Grup tempat bot memutar Musik/Radio.
6. `LOG_GROUP` : Grup untuk mengirim Daftar Putar, jika CHAT adalah Grup.
7. `ADMINS` : ID pengguna yang dapat menggunakan perintah admin.
8. `STREAM_URL` : URL streaming stasiun radio atau video langsung youtube untuk streaming saat bot dimulai atau dengan perintah /radio.
9. `MAXIMUM_DURATION` : Durasi maksimum lagu untuk diputar. (Opsional)
10. `REPLY_MESSAGE` : Balasan kepada mereka yang mengirim pesan ke akun USER di PM. Biarkan kosong jika Anda tidak membutuhkan fitur ini.
11. `ADMIN_ONLY` : Pass Y Jika Anda ingin membuat perintah /play hanya untuk admin CHAT. Secara default /play tersedia untuk semua.

- Aktifkan pekerja setelah menyebarkan proyek ke Heroku.
- Bot akan memulai radio secara otomatis di `CHAT` yang diberikan dengan `STREAM_URL` yang diberikan setelah penerapan. 
- Musik 24x7 bahkan jika heroku dimulai ulang, aliran radio dimulai ulang secara otomatis.  
- Untuk memutar lagu gunakan /play sebagai balasan file audio atau link youtube atau gunakan /play [nama lagu].
- Untuk mengunduh audio, Anda dapat menggunakan perintah [@SafoneMusicBot](http://t.me/SafoneMusicBot) atau `/song` ke bot.
- Gunakan `/help` untuk mengetahui tentang perintah lain & penggunaannya.

## Persyaratan

- Python 3.6 atau lebih tinggi.
- SEBUAH
  [Kunci API Telegram](https://docs.pyrogram.org/intro/quickstart#enjoy-the-api)
  dan akun Telegram.
- [FFmpeg Python](https://www.ffmpeg.org/)
- Telegram [Sesi String](http://t.me/genStr_robot) dari akun.
- Userbot Harus Menjadi Admin Di Channel atau Grup.
- Harus Memulai Obrolan Suara Di Saluran / Grup Sebelum Menjalankan Bot.

## Jalankan Di VPS (Jalan Sulit)

```sh
$ git clone -b V3.0 https://github.com/AsmSafone/RadioPlayer
$cd RadioPlayer
$ sudo apt-get install python3-pip ffmpeg
$ pip3 instal -U pip
$ pip3 install -r requirements.txt
# <buat variabel dengan tepat>
$ python3 main.py
```


## Lisensi
```sh
RadioPlayer, Bot Obrolan Suara Telegram
Hak Cipta (c) 2021 Asm Safone

Program ini adalah perangkat lunak gratis: Anda dapat mendistribusikannya kembali dan/atau memodifikasi
itu di bawah ketentuan Lisensi Publik Umum GNU Affero sebagaimana diterbitkan oleh
Free Software Foundation, baik versi 3 dari Lisensi, atau
(sesuai pilihan Anda) versi yang lebih baru.

Program ini disebarluaskan dengan harapan dapat bermanfaat,
tapi TANPA JAMINAN APAPUN; bahkan tanpa jaminan tersirat dari
DAGANG atau KESESUAIAN UNTUK TUJUAN TERTENTU. Lihat
Lisensi Publik Umum GNU Affero untuk lebih jelasnya.

Anda seharusnya telah menerima salinan dari GNU Affero General Public License
bersama dengan program ini. Jika tidak, lihat <https://www.gnu.org/licenses/>
```
