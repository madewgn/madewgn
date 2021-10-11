---
cover-img: https://telegra.ph/file/f9d7194946301649320bc.jpg
date: "2021-09-11T00:00:00Z"
share-img: https://telegra.ph/file/f9d7194946301649320bc.jpg
subtitle: Cara kompres video dengan ffmpeg
tags:
- ffmpeg
thumbnail-img: https://telegra.ph/file/f9d7194946301649320bc.jpg
title: Cara kompres video dengan ffmpeg
---

Tutorial Compress Video Dengan FFMPEG
Pada kesempatan kali ini saya akan memberikan tutorial compress video menggunakan ffmpeg, ffmpeg ini biasanya program yang digunakan aplikasi untuk compress video, salah satunya handbrake. Tutorial ini bisa dipakai di sistem operasi Linux dan Windows (disini saya menggunakan Linux, tetapi perintah nya sama saja mau Linux ataupun Windows)

Kalian install ffmpeg terlebih dahulu
Untuk Windows kalian bisa download di gyan.dev
untuk sistem operasi Linux saya sarankan menginstall ffmpeg dari snap, karena sudah support Hardware Accelerated, tetapi jika GPU kalian belum support NVENC kalian bisa menggunakan perintah

 ```sudo pacman -S ffmpeg (Arc based)```
 ```sudo apt install ffmpeg (Debian based)```

Jika kalian menggunakan snap bisa menggunakan perintah

 ```snap install ffmpeg```
Jika ffmpeg nya sudah terinstall kalian bisa cek menggunakan powershell atau terminal dengan perintah ```ffmpeg``` jika tidak muncul ```error``` berarti installasi selesai, jika muncul command not found berarti kalian belum setting PATH untuk ffmpeg nya,
Untuk setting PATH di Windows bisa kalian kunjungi sulhi.id
Untuk setting PATH di Linux kalian bisa kunjungi thread di stackoverflow
Sekarang kita mulai compress video nya dengan perintah
 ```ffmpeg -i input.mp4 -vcodec h264 -acodec aac output.mp4```
Jika kalian ingin menggunakan Hardware Accelerated, kalian bisa gunakan perintah
 ```ffmpeg -hwaccel cuvid -c:v h264_cuvid -i input.mp4 -c:v h264_nvenc -cq 19 -c:a copy output.mp4```
input.mp4 ini adalah nama dan extensi video yang akan di compress sedangkan output.mp4 adalah video yang sudah selesai di compress
-cq 19 0 itu auto 19 rekomendasi 51 lossless, kalian bisa pilih 1-51.