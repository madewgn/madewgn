---
image: "https://upload.wikimedia.org/wikipedia/commons/4/46/Google_Analytics_Logo_2015.png"
date: "2021-09-28T00:00:00Z"
share-img: https://upload.wikimedia.org/wikipedia/commons/4/46/Google_Analytics_Logo_2015.png
subtitle: Cara Menambahkan Google Analytics Pada Hugo
tags:
- blog
- jekyll
title: Cara Menambahkan Google Analytics Pada Hugo
---


Ketika kita mengelola sebuah website baik itu website pribadi, kantor, event, dll., pastinya kita ingin bisa memantau traffic dari website tersebut. Salah satu layanan gratis dari Google yang dapat membantu kita melakukan hal tersebut adalah Google Analytics.

Dengan Google Analytics, kita bisa mendapatkan informasi dari mulai halaman mana yang dikunjungi visitor, negara asal visitor, sumber dan kata kunci yang merujuk ke website kita, hingga pembuatan report tentang traffic dari website kita. Berbagai fungsi dari Google Analytics dibahas pada tautan berikut.

Hugo merupakan static website generator yang memungkinkan web developer untuk mengintegrasikan websitenya dengan Google Analytics. Jika sebelumnya Anda menggunakan Wordpress, Anda mungkin familiar dengan JetPack Plugin yang juga dapat diintegrasikan dengan Google Analytics. Pada Hugo, developer hanya perlu mengubah configuration file dari website untuk dapat menggunakan fungsi tersebut.

Berikut adalah tutorial untuk mengintegrasikan Hugo dengan Google Analytics.

Mendapatkan Tracking ID

Kunjungi https://analytics.google.com/.

Login dengan Google Account atau Gmail Account (@gmail.com). Jika belum memiliki Google Account, klik “Sign Up”.

Ikuti instruksi selanjutnya meliputi pembuatan akun Google Analytics, pemilihan layanan (Website, Apps, atau Apps dan Web, pilih Website), dan pendaftaran data website.

Setelah setup selesai, Anda akan mendapatkan Tracking ID dengan format ```UA-XXXXXXXXX-X.```

Mengubah Configuration File Hugo

Buka configuration file. Umumnya configuration file dapat ditemukan di root folder website Anda dengan nama ```config.toml.``` Akan tetapi, jika Anda menggunakan tema tertentu misalnya hugo-academic, config file tersimpan di ```config/_default/config.toml.```

Copy & paste Tracking ID seperti contoh berikut dengan Tracking-ID ```UA-XXXXXXXXX-X.```

```shell
[marketing] google_analytics = "UA-XXXXXXXXX-X" google_tag_manager = "" 
```

Jika Anda menggunakan hugo-academic, copy & paste Tracking ID seperti contoh berikut.

googleAnalytics = ```"UA-XXXXXXXXX-X"``` 

Save file tersebut kemudian lakukan commit dan push.

Final Check

Kunjungi website Anda dengan perangkat lain.

Kunjungi https://analytics.google.com/analytics/web/.

Buka bagian Reports - Realtime. Jika berhasil, seharusnya akan ditampilkan jumlah visitor yang sedang mengunjungi website Anda (minimal 1). Jika tidak, periksa kembali apakah ada langkah yang terlewat atau tunggu beberapa saat hingga website telah terupdate dengan ```config.toml``` yang terbaru.

