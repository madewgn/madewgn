---
title: "Lazy Bloggers Hugo themes"
date: 2021-10-07T04:26:53Z
tags: 
       - tema
image: "https://telegra.ph/file/eb406a9ab6f0ab494813b.jpg"
---


Halo kawan - kawan, selamat datang di blog saya, kali ini saya akan memberikan sebuah **tema Hugo** buatan saya sendiri 😂

## [DEMO](https://made-wiguna.web.app/)

{{< ads >}}

Saya memberikan nama **"Lazy-bloggers"**
Karena saya bukan seorang yang rajin:v

Tanpa basa-basi lagi langsung saya di pemasangan tema nya

Pertama silahkan buat dulu blog baru Hugo

```shell
hugo new site [nama web] -f yml
```
```shell
cd [nama web]
```
```shell
git clone https://github.com/MADEWGN/Lazy-bloggers themes/Lazy-bloggers
```
{{< ads >}}
Simple ``Config.yml``
```

baseurl: 'https://www.made-wiguna.web.app'
title: Lazy Bloggers
theme: Lazy-bloggers
googleAnalytics: UA-XXXXXX
disqusShortname: xxxxx

permalinks:
  post: '/blog/:slug/'
  page: '/:slug/'

params:
  author: admin
  description: 'Hello, Blog ini belum jadi. Sabar ya...'

frontmatter:
  date:
    - date
    - publishDate
    - lastmod
  lastmod:
    - ':git'
    - lastmod
    - date
    - publishDate
  publishDate:
    - publishDate
    - date
  expiryDate:
    - expiryDate

menu:
  main:
    - identifier: about
      name: About
      url: /about/
      weight: 1
    - identifier: art
      name: Home
      url: /
      weight: 2
    - identifier: Telegram
      name: Telegram
      url: 'https://t.me/[]/'
      weight: 3
    - identifier: github
      name: Github
      url: 'https://github.com/madewgn'
      weight: 4
```
Untuk membuat post baru
```shell
hugo new post/judul-post.md
```

Selamat mencoba 😄👋
{{< ads >}}
