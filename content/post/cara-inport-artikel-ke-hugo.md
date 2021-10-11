---
title: "Cara Inport Artikel blogger Ke Hugo"
date: 2021-09-30T22:20:29Z
image: "https://1.bp.blogspot.com/-z2_QdrUKmfE/WHx5QoVkwRI/AAAAAAAADok/AtwB9HQYNV4cxVuOFLlwgYCch_gi41rjQCK4B/s1600/tulisartikel-blogger-dan-hugo.jpg"
tags :
       - blog
       -  hugo
---

Dalam rangka migrasi blog saya yang sebelumnya di blogspot ke hugo, saya harus melakukan impor artikel dari Blogger ke Hugo.

Untungnya Hugo sudah menyediakan skrip untuk impor konten dari blogger ke Hugo.

Proses impor ini memakan waktu cukup cepat. Saya kira, tidak sampai 15 menit.

Mungkin anda bisa melakukannya lebih cepat.

Begini caranya…

{{< ads >}}

 pastikan telah menginstal Go (Golang) dan Git.
 
 ```shell 
 sudo apt install git golang
 ```

Kemudian lakukan langkah-langkah berikut ini.

{{< ads >}}


## 1. Ekspor Blog
Pertama, kita perlu mengekspor dulu konten yang ada di blogger. Masuk ke Settings>Other kemudian klik Back up Content

Kita akan mendapatkan file .xml, nah file ini nanti yang akan kita ekstrak isinya menjadi format markdown.

## 2. Download skrip
Selanjutnya kita membutuhkan skrip untuk melakukan ekstrak terhadap file .xml tadi. Silahkan klon skripnya di github.
```shell
git clone https://github.com/natefinch/blogimport
```
## 3. Impor Konten
Setelah kita mendapatkan skripnya, sekarang kita harus mengekstrak isi dari file .xml menjadi file markdown. Pertama, masuk dulu ke direktori skripnya.
```shell
cd blogimpor
```
{{< ads >}}


Setelah itu buat direktori baru sebagai tempat menampung hasil ekstraksi.
```shell
mkdir artikel 
```
Jalankan skrip:
```shell
go run main.go ~/Downloads/blog-2017-01-13.xml artikel 
```
Setelah itu, coba periksa direktori artikel.

Selanjutnya, kita bisa pindahkan semua file markdown ini ke direktori content di Hugo

