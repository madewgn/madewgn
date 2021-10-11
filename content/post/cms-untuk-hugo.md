---
title: "cara membuat CMS hugo dengan  Forestry.io"
date: 2021-10-10T03:30:39Z
tags: 
       - hugo
       - cms
image: "https://telegra.ph/file/c24b769e9fd69ea43b037.jpg"
---

Cara Setting Forestry.io Sebagai Post Editor Hugo

{{< ads >}}
Forestry.io adalah sebuah layanan software as a service (SaaS) yang berfungsi sebagai post editor untuk static site generator. Untuk menambah post (artikel) di static site generator hanya memakai text editor dan ditulis dalam syntax Markdown. Nah, dengan Forestry.io, menambah post tidak perlu lagi menggunakan text editor, melainkan editor dari Forestry.io atau biasa disebut dengan istilah WYSIWYG Editor.

{{< ads >}}
Forestry.io mendukung static site generator Hugo, Jekyll, VuePress, dan Gatsby. Layanan dari Forestry.io ini berbayar, namun tersedia juga paket Personal yang bisa digunakan tanpa biaya, selain itu kita dapat menambahkan website statis sebanyak mungkin (Unlimited sites).

Tutorial ini membahas tentang bagaimana cara setting atau menghubungkan Forestry.io dengan website Hugo yang sebelumnya sudah saya deploy ke GitLab Pages.

Menghubungkan Forestry.io dengan Hugo
Buat akun terlebih dahulu di Forestry.io.

Login, lalu klik Add Site.
![add site](/img/01.cara-setting-forestry-hugo_sites-forestry-min.jpg)
Belum ada website di Forestry.io

{{< ads >}}
Pilih static site generator Hugo, dan pilih versi. Versi yang terpasang di laptop Hugo v0.56.3, sementara versi paling tinggi di Forestry.io v0.56.1, ini tidak ada masalah, bisa berjalan dengan baik.

![pilih yang hugo](/img/02.cara-setting-forestry-hugo_select-static-site-generator-min.jpg)

Pilih di mana repository website Hugo berada, saya memakai GitLab.

{{< ads >}}

![pilih tempat host repo](/img/03.cara-setting-forestry-hugo_select-git-provider-min.jpg)

Tampil pertanyaan untuk mengijinkan Forestry.io mengakses akun GitLab, klik Authorize.

{{< ads >}}
![Authorize](/img/04.cara-setting-forestry-hugo_authorize-forestry-min.jpg)

Pilih nama repository tempat menyimpan website Hugo

Forestry.io mulai menjalankan importing site

{{< ads >}}
![import site](/img/06.cara-setting-forestry-hugo_importing-site-min.jpg)


Untuk menyelesaikan proses setup, klik Mark as done untuk Set up sidebar, Import media, dan Setup preview commands. Lalu klik Complete setup.

{{< ads >}}
![gambar 1](/img/08.cara-setting-forestry-hugo_finish-setup-process-min.jpg)

![gambar 2](/img/09.cara-setting-forestry-hugo_finish-setup-process-done-min.jpg)

{{< ads >}}
Selanjutnya buka menu Front matter dan klik Add Template.
Pada Create new template pilih Create based on existing document.

![buat template](/img/10.cara-setting-forestry-hugo_create-new-template-min.jpg)

Beri nama template dan pilih salah satu post yang sudah ada. Lalu klik Create Template

![beri nama](/img/11.cara-setting-forestry-hugo_add-template-min.jpg)

Hasil dari Create Template seperti di bawah ini.

![hasil](/img/12.cara-setting-forestry-hugo_template-fields-min.jpg)

Selanjutnya membuat Post, klik menu Post, Create new -> Post.

![Post](/img/13.cara-setting-forestry-hugo_posts-min.jpg)


{{< ads >}}
Masuk ke post editor, isi Title, Date, Tags, Categories, dan isi dari konten. Opsi Draft disamping tombol Save set Off jika ingin mempublikasi postingan yang dibuat.

![tulis artikel](/img/14.cara-setting-forestry-hugo_post-editor-min.jpg)

Setelah beberapa menit commit atau status pipeline passed, browsing URL dari website Hugo untuk melihat hasilnya.

Selamat mencoba 😄👍

{{< ads >}}
