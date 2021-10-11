---
comments: true
cover-img: https://www.transtv.co.id/layout/ttvnew/src/images/logo/01-ttv.png
date: "2021-07-17T00:00:00Z"
subtitle: cara membuat TV online trans 7  di blog atau website
tags:
- javascript
- Blogger
thumbnail-img: https://www.transtv.co.id/layout/ttvnew/src/images/logo/01-ttv.png
tittit: cara membuat TV online di blog atau website
---

## cara membuat TV online trans 7 di blog atau website

Cara Mudah Memasang Script Streaming TV Online di Blog – Tutorial kali ini saya akan membagikan bagaimana cara memasang script streaning TV Online di blog.

Sebenarnya cara memasangnya cukup mudah, yang perlu anda lakukan adalah mencari embed TV Online itu sendiri kemudian anda pasangkan di blog anda.

 

>Anda tidak perlu pusing untuk mencarinya, dibawah ini sudah saya sertakan script embednya, jadi anda tinggal memasangnya saja di Blog anda.

>Streaming TV Online ini sangat cocok untuk anda yang suka nonton tv dari internet dan memudahkan orang lain ketika dalam perjalanan di kendaraan umum untuk menonton acara favoritnya di tv.

 


Online TV Streaming

Jika sudah banyak orang yang tahu bahwa dalam blog anda terdapat Streaming TV Online, pasti mereka akan kembali lagi ke blog anda jika ingin menonton tv, sehingga akan menambah pengunjung tetap di blog anda.

Lalu bagaimana cara membuat blog TV Online di platform Blogger atau blogspot? saya akan memberikan sedikit tutorial mengenai cara memasang embed/script streaming tv online :

Panduan Memasang Embed/Script Streaming TV Online


1. Pertama login terlebih dahulu ke akun blogger anda

2. Buat postingan baru atau bisa juga pada halaman statis (Page) blog anda

3. Selanjutnya Buat Judul berdasarkan stasiun tv, misal kita akan Membuat channel RCTI, maka anda bisa menamainya dengan “RCTI Live Streaming”

4. Pada kolom postingan pilih tab HTML, ingat HTML bukan Compose ya!

5. Selanjutnya pilih salahsatu script dibawah ini, paste ke dalam postingan anda :

Embed/Script Streaming TV Online

<div style="background-color: #2c323c; border-radius: 0px 15px; padding: 17px; text-align: left;"> <span style="color: white; font-family: 'Fira Mono', monospace; font-size: 15px;">&lt;div id="MadeWiguna-trans7">&lt;/div&gt;
&lt;script&gt;
  var f = document.createElement("iframe");
  f.src = "https://madewiguna.netlify.app/proyek/trans7.html";
  f.width = "100%";
  f.height = 380;
  f.scrolling = "no";
  f.frameBorder = 0;
  var rootEl = document.getElementById("MadeWiguna-trans7");
  console.log(rootEl);
  rootEl.appendChild(f);
&lt;/script&gt;</span></div>


# live demo

<div id="MadeWiguna-trans7"></div>
<script>
  var f = document.createElement("iframe");
  f.src = "https://20.detik.com/watch/livestreaming-trans7";
  f.width = "100%";
  f.height = 380;
  f.scrolling = "no";
  f.frameBorder = 0;
  var rootEl = document.getElementById("MadeWiguna-trans7");
  console.log(rootEl);
  rootEl.appendChild(f);
</script>
