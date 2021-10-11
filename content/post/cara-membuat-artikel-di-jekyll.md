---
title: "Cara Membuat Artikel Di Jekyll"
date: 2021-10-01T04:06:19Z
image: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTwjrAEEhW_HD6FLnHtacdVvbRAXdYaw01qYw&usqp=CAU"
tags:
       - blog
       - jekyll
---

Halo selamat datang kembali di **Made Wiguna  project** disini saya akan membahas bagaimana sih caranya membuat artikel jekyll

{{< ads >}}

Buat yang belum tahu cara membuat blog dengan jekyll bisa di baca di sini ya 
[https://madewgn.github.io/artikel/cara-nge-blog-dengan-jekyll/](https://madewgn.github.io/artikel/cara-nge-blog-dengan-jekyll/)

Btw ada dua cara nih untuk menulis di jekyll, yang pertama menulis langsung dari github / gitlab yang kedua menulis secara offline di text editor. Sekarang saya akan membahas dua-duanya nih, tapi yang pertama akan saya bahas adalah cara menulis artikel langsung dari github

{{< ads >}}

## cara menulis langsung dari github

Jika kalian sudah login ke akun github kalian sekarang silakan dipilih nama repository blog kalian (contoh **github.com/[username]/[username].github.io**)

Jika sudah login sekarang buka folder ```_post``` pada repository kalian.

Setelah itu buat file baru dengan format

```shell
2014-3-12-Hello-World.md
```
```shell
Keterangan :
           - 2014 = Tahun artikel di buat
           - 3 adalah bulan saat artikel nya di buat
           - 12 adalah tanggal saat artikel nya di buat
           -  Hello-World adalah judul artikel nya
 ```

Jangan lupa di akhiri dengan .md karena file nya berformat markdowns

{{< ads >}}

Sekaran kita akan belajar struktur post di jekyll

Contoh :

```shell

---
layout: post
title: saya sedang belajar membuat post di jekyll
---

Ini adalah isi artikel nya

```


Nah seperti itu. Untuk menambah kan foto / gif nya juga cukup mudah, lebih mudah dari html

Contoh 

```shell
![Contoh gambar]( di sini isi link gambar)

```

{{< ads >}}


Dan hasilnya akan seperti ini
 ![contoh](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTwjrAEEhW_HD6FLnHtacdVvbRAXdYaw01qYw&usqp=CAU)
 
 
 ## cara nulis artikel offline
 
 {{< ads >}}
 
 Langkah pertama pastikan di komputer kalian sudah terinstall git
 
 Jika belum silahkan di install dulu, saya sarankan untuk ngeblog offline buat yang jaringan internet nya kurang lancar 😅
 
 Saya sendiri nge blog nya di HP, tapi saya menggunakan, hugo.
 
 Pertama silahkan clone repo github kalian, dengan cara
 
 ```shell
 
 git clone https://github/[username]/[username].github.io/
 
 ```
 
 Setalah itu buka text editor dan buat file baru dengan format markdowns (.md)
 
 Untuk struktur dan cara membuat artikelnya tetap sama seperti yang di atas sekian tutorial dari saya semoga bermanfaat jika ada yang ditanyakan bisa dm saya di telegram [@madewgn](t.me/madewgn)
 
 {{< ads >}}
 




