---
title: "Cara Migrasi WordPress Ke Hugo"
date: 2021-10-02T02:23:34Z
image: "https://d33wubrfki0l68.cloudfront.net/a061f480415247b6d2d7f82c798dbf895670e7a5/85d79/assets/fromwordpresstohugo.png.webp"
tags:
       - blog
       - hugo
       - wordpress
---

## cara migrasi WordPress ke  Hugo

Selamat datang lagi di blog madewgn dulu saya sudah pernah membahas bagaimana caranya migrasi blogger ke hugo tapi sekarang saya akan memberikan tutorial singkat bagaimana sih caranya migrasi dari wordpress ke hugo.
{{< ads>}}
Pertama - tama silakan Install python terlebih dahulu

```shell
sudo apt-get install python-yaml python-bs4 python-html2text
```
Langkah kedua silakan clone dulu repository nya

```shell
git clone https://github.com/wooni005/exitwp-for-hugo.git
```
 {{< ads>}}
Silakan taruh file ```.xml``` wordpress nya di dalam direktori ```wordpress-xml```

Lalu kitik kan perintah

```shell
sudo pip install --upgrade -r pip_requirements.txt
```
```shell
sudo apt-get install libyaml-dev python-dev build-essential
```

Untuk menjalankan kode nya cukup  ketikkan perintah
```shell
./exitwp.py
```
Dokumentasi selengkapnya : https://github.com/wooni005/exitwp-for-hugo

[Tutorial hugo lainnya](/artikel/tutorial-hugo-lengkap/)

{{< ads>}}
