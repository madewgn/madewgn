---
cover-img: https://telegra.ph/file/083ee09d368e0ee991996.jpg
date: "2021-09-01T00:00:00Z"
share-img: https://telegra.ph/file/083ee09d368e0ee991996.jpg
subtitle: Cara deploy userge di termux atau localhost
tags:
- Telegram
- userbot
- bot
thumbnail-img: https://telegra.ph/file/083ee09d368e0ee991996.jpg
title: Cara deploy userge di termux
---

# Panduan Termux untuk Pengguna

<pre><b>Penting!</b> tidak seperti heroku, semuanya akan dikenakan biaya dari Anda</pre>

## Prasyarat

* Aplikasi [Termux](https://play.google.com/store/apps/details?id=com.termux)
* Setidaknya penyimpanan perangkat **750MB**

## Pengaturan Cepat

* Buka Termux dan jalankan `bash <(curl -s https://theuserge.github.io/termux.sh)`.
* Tunggu beberapa saat (`hingga 10 menit`) ... (beberapa kali mungkin meminta input).
* Ini akan mengarahkan ke `config.env` dan meminta untuk mengisi.
* Isi, simpan (`ctrl+s`) dan tutup (`ctrl+x`).
* Sekarang, Instalasi selesai dan waktu untuk menjalankan userge.
* Tapi pertama-tama lakukan `termux-chroot` untuk memperbaiki masalah DNS Resolver.
* Bagus, Sekarang Anda berada di root jadi `cd Userge && bash run`.
* Menikmati :)

## Selangkah demi selangkah:

Pertama-tama, Perbarui paket dan Instal Repositori root

```bash
pembaruan pkg && peningkatan pkg
pkg instal root-repo
```

Instal Python dan paket yang diperlukan

```bash
pkg instal python
pip install -U pip wheel setuptools
pkg instal git jq proot resolv-conf libxml2 libxslt libjpeg-turbo
```

Pasang Bantal

```bash
LDFLAGS="-L/system/lib/" CFLAGS="-I/data/data/com.termux/files/usr/include/" pip install Bantal
```

Kemudian Klon `Pengguna` dan Buka direktori kloning

```bash
git clone https://github.com/UsergeTeam/Userge Userge && cd Userge
```

Persyaratan Instal

```bash
CFLAGS="-O0" pip install -r requirements.txt
```

Hasilkan dan Isi `config.env`

```bash
cp config.env.contoh config.env
nano config.env
```

Selesai. Sekarang jalankan Userge

```bash
termux-chroot
cd pengguna
lari bash
```