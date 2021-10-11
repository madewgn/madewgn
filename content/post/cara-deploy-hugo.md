---
title: "Cara Deploy Hugo ke github"
date: 2021-10-04T22:28:20Z
image: "https://telegra.ph/file/ae891af3c31582bb1891e.jpg"
tags:
      - hugo
      - github
---

Melanjutkan tulisan sebelumnya mengenai cara membuat blog dengan Hugo, sekarang kita akan menghostingkan static site yang kita buat ke Github. Dengan fitur Github Pages yang disediakan oleh Github, kita bisa menghostingkan file-file yang digenerate oleh Hugo.
{{< ads >}}
Pertama, buat terlebih dahulu sebuah repository di Github.

Sebagai contoh, saya sudah membuat repository dengan alamat berikut:

https://github.com/madewgn/madewgn.github.io/
{{< ads >}}
Kemudian, buatlah 2 branch, yaitu main dan pages.

Branch main nantinya akan digunakan sebagai menyimpan source dari file-file Hugo kita. Sedangkan branch pages digunakan untuk menyimpan hasil static site dari Hugo.

Push terlebih dahulu source project dari Hugo ke branch ``main.``

Setelah itu generate static site dari Hugo dengan command ``hugo.``
{{< ads >}}
Pindah ke directori public, kemudian buat repo untuk dimasukkan ke Github dengan branch pages dengan cara berikut.
```
> cd public 
> git init 
> git add . 
> git commit -m "first commit" 
> git branch -m pages 
> git remote add origin https://github.com/<username>/<project>.git
> git push -u origin pages 

```
Langkah terakhir yaitu mengaktifkan fitur Pages di Github
{{< ads >}}
Untuk mengaktifkan fitur Github Pages cukup mudah.

Pertama, kalian cukup buka menu Settings yang ada di bagian kanan repositori kalian.

Kemudian, di bagian bawah akan ada sub-menu dengan nama Github Pages.

Pilih branch pages yang merupakan HTML dari static site yang ter-generate.

Lalu Save
![aktif kan github pages](https://www.kangsunu.com/cara-hosting-deploy-hugo-di-github/3-enable-github-pages.gif)

Sekarang blog yang dibuat dengan Hugo sudah bisa diakses dengan alamat ****https://<username>.github.io/<project>.**** Pada tulisan ini, maka contoh blog yang saya buat diakses melalui ****https://madewgn.github.io/.**** Bila ingin menggunakan domain root dari Github, maka nama repositori yang dibuat harus ****<username>.github.io.**** Untuk akun Github saya jadinya ****madewgn.github.io.****

{{< ads >}}
