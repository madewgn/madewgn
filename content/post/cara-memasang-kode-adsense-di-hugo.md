---
title: "Cara Memasang Kode Adsense Di Hugo"
slug: cara-memasang-kode-adsense-di-hugo
date: 2021-10-05T10:17:25Z

type: post

tags:
    - hugo

image: "https://telegra.ph/file/4c0ccf68d91c3fbb93565.jpg"
description: ""

typora-root-url: ../../static
typora-copy-images-to: ../../static/img/cara-memasang-kode-adsense-di-hugo/
---

![ads](https://telegra.ph/file/4c0ccf68d91c3fbb93565.jpg)

Halo selamat datang kembali di Made Wiguna Bloggers, kali ini saya akan memberikan tutorial singkat cara memasang kode AdSense di  hugo, tapi sebelum itu pastikan kamu sudah mempunyai akun adsense nya dulu ya !! :D

Btw ada 2 cara nih untuk menampilkan iklan AdSense di hugo
1. Pasang script AdSense di ```head.html```
2. Menggunakan shortcode

Yang pertama akan saya bahas ada cara menambahkan script AdSense di ``head.html``

Silakan login ke akun AdSense kalian, setelah itu salin kode AdSense nya


Contoh kode :
```shell
<!-- google adsense -->
<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-XXXXXXXXXXXXXX"
     crossorigin="anonymous"></script>
```
Kemudian buka direktori ``themes/[NAMA TEMA MU]/layouts/partials/head.html``

Sekarang tinggal paste aja script nya di sana.


Metode ke 2
 Cara memasang kode AdSense dengan shortcode,
 Dengan menggunakan cheat kode kayan bisa mengatur sendiri di mana keinginan kalian meletakkan iklannya (di dalam artikel)
 
 Contoh nya saya akan menaruh iklan tepat di bawah tulisan ini
 
{{< ads >}}


Gimana ada kan?😄

Untuk cara membuat nya pun sangat mudah, 

Silakan buat shortcode baru dengan nama ``ads.html`` dalam direktori ``themes/[NAMA TEMA MU]/layouts/shortcode/``

Untuk mendapatkan kode nya silahkan login ke akun AdSense kalian, setelah itu pilih menu ``iklan`` , lalu buka `menurut unit iklan` , dan buat `iklan dalam artikel`

Copy semua kode yang di berikan dan paste kan di ``ads.html (dalam shortcode)``

Nah sekarang tinggal tinggal tambahkan kode
Dalam artikel mu

![ads](https://telegra.ph/file/5435fc67f7b7ae50145c9.jpg)

Hasilnya akan seperti ini

{{< ads >}}

Nah seperti itu, dengan shortcode iklan AdSense bisa kamu taruh sesuai selera 
Selamat mencoba

Jika mengalami kesulitan silahkan hubungi saya di Telegram
