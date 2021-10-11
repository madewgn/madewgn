---
date: "2021-09-27T00:00:00Z"
image: "https://i1.wp.com/codelatte.org/wp-content/uploads/2018/11/github-jekyll.png"
subtitle: cara nge blog dengan jekyll
tags:
- blog
- jekyll
title: cara nge blog dengan jekyll
---

## Membuat Blog di GitHub Menggunakan Jekyll 

Jekyll adalah generator situs web yang dirancang untuk membuat blog statis untuk di-hosting di Halaman GitHub. Tom Preston-Werner menciptakan Jekyll untuk memungkinkan orang untuk blog menggunakan situs HTML statis sederhana, dengan semua konten yang di-host dan dikendalikan oleh versi di GitHub. Tujuannya adalah untuk menghilangkan kerumitan platform blog dengan membuat alur kerja yang memungkinkan blogging dengan cara yang lebih sederhana.

## Bagaimana Cara Kerja Jekyll?

Dikutip dari situs resmi nya, Jekyll memungkinkan kita untuk membuat blog dengan mudah dan tanpa menggunakan database. Semua halaman dan post akan diubah menjadi HTML Statis sehingga mempercepat loading karena tidak perlu memanggil database.

Jekyll mengambil konten kita yang ditulis dalam Markdown, memberikannya melalui template dan menerapkannya sebagai situs web statis, siap untuk disajikan. GitHub Pages dengan mudah melayani situs web langsung dari repositori GitHub kita, sehingga kita tidak perlu berurusan dengan hosting apa pun.





Pada artikel kali ini kita akan belajar membuat blog di Github Pages menggunakan Jekyll. Proses kali ini akan sedikit lebih sederhana daripada yang lain, karena kita hanya akan melakukan 4 step, diantaranya adalah:

1.Membuat blog dari Jekyll.

2.Meng-hostingkan blog Jekyll kita secara gratis di GitHub.

3.Mengedit/mengcustom blog seperti nama, avatar dan link social media.
Publikasikan post pertama kita!

4. Publikasikan post pertama kita!

## Membuat Blog di GitHub Menggunakan Jekyll

note : jika belum punya akun github silakan di buat dulu.


Kunjungi [Jekyll Now](http://www.github.com/barryclark/jekyll-now), dan tekan tombol “Fork” di sudut kanan atas repositori untuk menyalin salinan tema blog ke akun GitHub kalian.

![contoh](https://i0.wp.com/cloud.netlifyusercontent.com/assets/344dbf88-fdf9-42bb-adb4-46f01eedd629/cddcf942-6cc7-4a1f-bf1b-5066b5e553ec/step1.gif)

Sebagai pengguna GitHub, kita berhak atas satu situs web “pengguna” gratis, yang akan ditayangkan di ```http://usernamegithub.github.io.``` Ruang ini sangat ideal untuk hosting blog Jekyll! Selanjutnya kita perlu mengganti nama repository yang sudah kita Fork tadi menjadi ```usernamegithub.github.io.```

![gambar](https://i1.wp.com/codelatte.org/wp-content/uploads/2018/11/Screen-Shot-2018-11-01-at-8.12.45-PM.png)

Situs web kalian akan segera ditayangkan. Kalian dapat memeriksa dengan membuka ```http://usernamegithub.github.io``` kalian

![hasil](https://i0.wp.com/codelatte.org/wp-content/uploads/2018/11/Screen-Shot-2018-11-01-at-8.15.18-PM.png)


## Kustomisasi Blog Jekyll

Sekarang kalian dapat mengubah nama situs web, deskripsi, avatar, dan opsi lainnya dengan mengedit file ```_config.yml.``` Variabel khusus ini telah sudah untuk kenyamanan saat situs web Anda dibuat.

Membuat perubahan ke ```_config.yml``` (atau file apa pun dalam repositori kalian) akan memaksa Halaman GitHub untuk membangun kembali situs web kalian dengan Jekyll. Situs web yang dibangun kembali akan dapat dilihat beberapa detik kemudian di ```http://usernamegithub.github.io.``` 



