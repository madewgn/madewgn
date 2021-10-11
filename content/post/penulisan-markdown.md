---
title: "panduan menulis mengunakan markdowns"
date: 2021-10-01T10:46:30Z
image: "https://telegra.ph/file/2f5e8397e1586b42d262b.jpg"
tags:
       - markdown
---

{{< ads >}}

Bagi yang sering bermain di Github dan web serupa, pasti sering melihat markdown. Biasanya markdown digunakan untuk menuliskan dokumentasi.

Pada dasarnya markdown sama seperti HTML. Namun, lebih sederhana dan mudah dibaca.

Saat ini markdown sudah digunakan untuk:

* Dokumentasi;

* SSG (Static Site Generator);

* CMS seperti Ghost, Wordpress, Tumblr, dll.;

* Penulisan Buku;

* Format teks pada chat: Telegram, WA, Facebook;

* dll.
{{< ads >}}
Pada kesempatan ini, kita akan belajar dasar-dasar format markdown hingga format tingkat lanjut.


Apa itu Markdown?

Markdown adalah (lightweight markup language) bahasa markup yang lebih ringan dari HTML untuk formatting teks.

Markdown bisa dikonversi ke dalam HTML menggunakan beberapa aplikasi. Biasanya menggunakan markdown editor itu sendiri.

Markdown dibuat pada tahun 2004 oleh John Gruber. Tujuannya untuk mempermudah penulisan dokumen web—mudah ditulis dan mudah dibaca—Karena menulis langsung HTML terasa melelahkan dan susah dibaca.

Contoh:

```shell
Aku *sedang* belajar **menulis** dengan [markdown](https://en.wikipedia.org/wiki/Markdown). 
```
Teks ini akan dikonversi ke HTML menjadi seperti ini:

Aku sedang belajar menulis dengan markdown.
{{< ads >}}
```shell
Aku <em>sedang</em> belajar <strong>menulis</strong> dengan <a href="https://en.wikipedia.org/wiki/Markdown">markdown</a>. 
```

Menurutmu mana yang lebih mudah ditulis?

Pasti banyak yang akan menjawab markdown.

Saya sendiri sudah merasakan perbedaannya.

Waktu menulis di Blogger, saya menulis langsung HTML di setiap artikel. Rasanya melelahkan 😫…

Ketika sudah mirgrasi ke Hugo, saya menulis dengan markdown dan terasa lebih cepat dan produktif dibandingkan HTML.

{{< ads >}}
File Markdown
File markdown dapat kita simpan dengan ekstensi .markdown atau .md.

Contoh: belajar-menulis.md atau belajar-menulis.markdown

Format dasar Markdown
Sekarang mari kita coba menulis format-format dasar markdown. Pertama, mari kita mulai dari:

Membuat Heading
Heading atau judul di markdown dapat dibuat dengan tanda pagar #.
{{< ads >}}
Contoh:
```shell
# Heading 1
## Heading 2
### Heading 3
```
Maka akan menghasilkan:
```shell
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
```
Heading ini sampai level 6 seperti pada HTML. Jumlah tanda pagar di depannya menandakan levelnya.

Selain menggunakan tanda pagar, ada juga yang menggunakan simbol minus (-) dan samadengan (=) seperti ini:
```shell
Ini Headeing Level 1
====================

ini paragraf, bla bla bla...

Ini heading level 2
-------------------

ini paragraf, bla bla bla...
```
## Format Teks

{{< ads >}}
Format Teks

Jika kamu ingin menulis teks tebal, miring, dan strikeline, maka bisa dilakukan seperti ini:
```shell
**Tebal** *miring* ~~strikeline~~ 
```

Selain menggunakan tanda bintang, untuk teks tebal dan miring bisa juga menggunakan garis bawah (underscore) seperti ini:
```shell
__teks tebal__ _teks miring_ 
```

Membuat Link

Link dapat kita buat dengan tanda kurung seperti ini:

```shell
[Made Wiguna project](https://madewgn.github.io/) 
```

Hasilnya:

[Made Wiguna project](https://madewgn.github.io/)

Kita juga bisa menambahkan title untuk tooltips:
```shell
[Made Wiguna project](https://madewgn.github.io/ "Pergi ke made Wiguna project") 
```

Hasilnya:

[Made Wiguna project](https://madewgn.github.io/ "Pergi ke made Wiguna project") 

Selain menggunakan tanda kurung, kita juga bisa membuat link langsung dengan menuliskan URL lengkapnya.

Contoh:

https://en.wikipedia.org/wiki/Markdown 

Maka akan menghasilkan:

https://en.wikipedia.org/wiki/Markdown



{{< ads >}}



