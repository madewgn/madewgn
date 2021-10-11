---
title: "Pejuang Hugo Themes"
date: 2021-10-09T11:37:31Z
image: "https://telegra.ph/file/92fc86006b35daf828bd1.jpg"
tags:
       - tema hugo
---


Yo halo, welcome back 😄👋
Kali ini saya mencoba tema Hugo baru nih yang saya beri nama "pejuang" ya pejuang sangat cocok buat kalian yang sedang berjuang di dunia blogging...
{{< ads >}}
Tema cocok bua kalian yang suka blog dengan tampilan sederhana, btw tema hugo satu ini sangat muda untuk di modif, jadi sangat mudah jika kamu ingin nambahin beberapa kode di tema ini
{{< ads >}}

Btw di tema ini saya tambahin fitur list artikel terbaru,jadi nya kaya blogspot 
![demo](https://telegra.ph/file/85995665a8b9f8a042cc1.jpg)


## [DEMO](https://pejuang-hugo.netlify.app)

Cara menggunakan themes nya

{{< ads >}}

```shell
hugo new site [nama web] 
```
```shell
cd [nama web]/themes
```
```shell
git clone https://github.com/MadeWGN-GIT/pejuang-hugo
```
{{< ads >}}
Simple ``Config.toml``

```
title = "MADE WIGUNA"
baseurl = "https://madewgn.github.io/"

# Agar front-matter pakai format YAML
MetaDataFormat = "yaml"

# untuk apply temanya
themesDir = "themes"
theme = "pejuang-hugo"

# Shortname disqus, silahkan sesuaikan
DisqusShortname = "XXX"

# Untuk Google Analytic, silahkan sesuikan
googleAnalytics = "UA-XXXXXXXX"

# Untuk deskripsi tag meta di homepage
description = "Blog pengguna HP"

# Biodata Author
[author]
    name = "Made Wiguna"
    homepage = "https:t.me/madewgn/"
    bio = "Pengamat Langit"
    image = "https://telegra.ph/file/3a7fbe5e09b173a369511.jpg"

```
Untuk membuat post baru
```shell
hugo new post/judul-post.md
```
Selamat mencoba 😄👋


{{< donasi >}}


{{< ads >}}
