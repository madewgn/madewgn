---
comments: true
cover-img: https://2.bp.blogspot.com/-7UvPy_O6cPs/VCQ0h-ife0I/AAAAAAAAGfU/dMrmAptj8yQ/s1600/radio%2Bonline%2Bmy%2Bradio%2Bstream%2Bembed%2Bplayer.png
date: "2021-07-19T00:00:00Z"
subtitle: cara membuat Radio online di blog atau website
tags:
- javascript
- Blogger
thumbnail-img: https://2.bp.blogspot.com/-7UvPy_O6cPs/VCQ0h-ife0I/AAAAAAAAGfU/dMrmAptj8yQ/s1600/radio%2Bonline%2Bmy%2Bradio%2Bstream%2Bembed%2Bplayer.png
tittit: cara membuat Radio online di blog atau website
---


PUNYA Radio Online Streaming alias Radio Internet di My Radio Stream? Mau pasang alias "tempel" (embed) playernya di blog blogspot Anda?

Oh, blom punya? Bikin dong, gratis kok! Ini dia Cara Membuat Radio Online.

Kalau sudah punya, untuk memasang playernya di blog, Anda tinggal COPY kode berikut ini dan PASTE di Halaman Statis atau di Sidebar (Widget).


>Cara memasang Player Radio Online di Halaman Statis (Static Page):
>1. Pages > New Page > Klik mode "HTML"
>2. COPAS kode berikut ini:


<div style="background-color: #2c323c; border-radius: 0px 15px; padding: 17px; text-align: left;"> <span style="color: white; font-family: 'Fira Mono', monospace; font-size: 15px;">&lt;div id="MadeWiguna-trans7">&lt;/div&gt;
&lt;script&gt;
  var f = document.createElement("iframe");
  f.src = "https://madewgn.github.io/Proyek/Radio.html";
  f.width = "100%";
  f.height = 380;
  f.scrolling = "no";
  f.frameBorder = 0;
  var rootEl = document.getElementById("MadeWiguna-trans7");
  console.log(rootEl);
  rootEl.appendChild(f);
&lt;/script&gt;</span></div>

## live demo

<div id="MadeWiguna-trans7"></div>
<script>
  var f = document.createElement("iframe");
  f.src = "https://madewgn.github.io/Proyek/Radio.html";
  f.width = "100%";
  f.height = 380;
  f.scrolling = "no";
  f.frameBorder = 0;
  var rootEl = document.getElementById("MadeWiguna-trans7");
  console.log(rootEl);
  rootEl.appendChild(f);
</script>


