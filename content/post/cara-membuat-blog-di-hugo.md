---
title: "Cara Membuat Blog Di Hugo"
date: 2021-10-01T10:22:48Z
image: "https://telegra.ph/file/868c5fb52501b0b195240.jpg"
tags:
       - hugo
       - blog
---

Sebelumnya sudah saya buat persiapan ngeblog di hugo sekarang akan saya buatkan tutorial cara membuat blog di hugo lengkap dengan cara membuat artikelnya

{{< ads >}}

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

```shell

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
```shell
nano config.toml
```
selain dengan nano kamu juga dapat mengedit nya dengan teks Editor.
dan ganti semua kode nya, langsung simpan

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

{{< ads >}}

![baru selesai di buat](https://res.cloudinary.com/practicaldev/image/fetch/s--yyLdc3MQ--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/0s4okm8z8whiojeex4ba.jpg)

## Menulis artikel di Hugo
Pertama, buatlah sebuah artikel.
```shell
hugo new post/judul-artikel.md
```
Setelah itu, edit artikel menggunakan teks editor.
Setelah mengeditnya, jalankan 
```shell
hugo server
```
 untuk melihat artikel.
 
 Hasilnya akan terlihat seperti ini
 
 ![hasil akhir ](https://res.cloudinary.com/practicaldev/image/fetch/s--NIRLAMWv--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/gj58su7z23lozsv3llk5.jpg)
 
 Apa selanjutnya? 
 Selanjutnya adalah [belajar penulisan markdowns yang benar](/artikel/panduan-menulis-mengunakan-markdowns/)
 
 {{< ads >}}
