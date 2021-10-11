---
image:  "https://telegra.ph/file/868c5fb52501b0b195240.jpg"
date: "2021-10-02T00:00:00Z"
share-img: https://telegra.ph/file/868c5fb52501b0b195240.jpg
subtitle: cara mudah nge blog dengan hugo
tags:
- hugo
- blog
thumbnail-img: https://telegra.ph/file/868c5fb52501b0b195240.jpg
title: Cara NgeBlog di HP dengan hugo
---

## Memang bisa ngeblog pakai Termux?

Tentu saja bisa dong, membahas Termux tidak melulu tentang hacking dan sebagainya.

Banyak hal yang bisa kalian manfaatkan dari Termux ini, salah satunya untuk ngeblog.

Supaya bisa ngeblog di Termux, kalian bisa menggunakan static site generator, alat yang berfungsi untuk membangun website statis.

Website statis sudah aja sejak dulu, sebelum adanya CMS (WordPress, Joomla, Drupal, dll).

Dulu untuk membangun situs web statis, perlu membuat satu per satu file HTML, CSS, dan JavaScript.
{{< ads >}}
Namun, sekarang sudah ada alat yang jauh lebih canggih untuk membangun website statis, salah satunya static site generator.

Sehingga tidak perlu lagi mengedit satu per satu file HTML, CSS, dan JavaScrip untuk mengubah website.

Cara kerja static site generator, yaitu dengan membuat file statis (HTML, CSS, dan JavaScript) dari template dan konten.

Saat ini sudah ada banyak sekali static site generator, yaitu Jekyll, Hugo, Hexo, GatsbyJS, dsb.

Dalam pembahasan kali ini, aku memakai Hugo.

{{< ads >}}

##Instalasi Hugo di Termux

Jalankan perintah ini untuk menginstal hugo dan git di Termux
```shell
pkg install hugo git
```
Setelah semuanya terinstal, mari mulai ngeblog dengan Hugo pakai Termux!

Membuat blog dengan Hugo
Pertama, buatlah blog dengan hugo seperti contoh berikut ini.
```shell
hugo new site namablog
```
Kedua, masuk ke direktori namablog.
```shell
cd namablog
```
Selanjutnya, unduh tema dan pasang ke blog kalian.

Temanya bisa kalian unduh dari Hugo Themes.

Baca dulu dokumentasi temanya karena di sana ada konfigurasi yang harus diikuti supaya tema bisa digunakan.

Sebagai contoh, aku menggunakan tema hugo-theme-terminal.

Maka konfigurasi config.toml yang diperlukan seperti berikut ini.

{{< ads >}}

```

baseurl = "/"
languageCode = "en-us"
theme = "terminal"
paginate = 5

[params]
  # dir name of your blog content (default is `content/posts`)
  contentTypeName = "posts"

  # ["orange", "blue", "red", "green", "pink"]
  themeColor = "orange"

  # if you set this to 0, only submenu trigger will be visible
  showMenuItems = 2

  # show selector to switch language
  showLanguageSelector = false

  # set theme to full screen width
  fullWidthTheme = false

  # center theme with default width
  centerTheme = false

  # set a custom favicon (default is a `themeColor` square)
  # favicon = "favicon.ico"

  # set all headings to their default size (depending on browser settings)
  # it's set to `true` by default
  # oneHeadingSize = false

[languages]
  [languages.en]
    languageName = "English"
    title = "Aditya Phra Blog"
    subtitle = "Seorang penulis dan penggemar Linux"
    keywords = ""
    copyright = ""
    menuMore = "Show more"
    readMore = "Read more"
    readOtherPosts = "Read other posts"

    [languages.en.params.logo]
      logoText = "Aditya Phra Blog"
      logoHomeLink = "/"

    [languages.en.menu]
      [[languages.en.menu.main]]
        identifier = "about"
        name = "About"
        url = "/about"
      [[languages.en.menu.main]]
        identifier = "showcase"
        name = "Showcase"
        url = "/showcase"
        
        
```
untuk mengubah config.toml kamu hanya perlu memberikan perintah
```nano config.toml```
dan ganti semua kode nya, untuk menyimpan takan crlt + x terus Y lalu enter

{{< ads >}}

Kloning tema terminal ke direktori themes blog.

```shell
git clone https://github.com/panr/hugo-theme-terminal themes/terminal
```
Selanjutnya, uji coba blogmu dengan hugo server.
```shell
hugo server
```
Terakhir, akses alamat blog (http://localhost:1313) melalui bbrowser

![pic](https://res.cloudinary.com/practicaldev/image/fetch/s--yyLdc3MQ--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/0s4okm8z8whiojeex4ba.jpg)

## Menulis artikel di Hugo
Pertama, buatlah sebuah artikel.
```shell
hugo new posts/judul-artikel.md
```
Setelah itu, edit artikel menggunakan teks editor.
```shell
nano content/posts/judul-artikel.md
```
Kalian bisa menggunakan markdown sebagai format penulisan artikel.

Setelah mengeditnya, jalankan 
```shell
hugo server
``` 
untuk melihat artikel.

{{< ads >}}

![pic2](https://res.cloudinary.com/practicaldev/image/fetch/s--NIRLAMWv--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/gj58su7z23lozsv3llk5.jpg)

{{< ads >}}

Selamat Blog kamu dengan hugo sudah jadi !
