---
comments: true
date: "2021-07-14T00:00:00Z"
subtitle: Cara membuat teks Editor dengan HTML dan java script
tags:
- html
- JavaScript
title: Cara membuat teks Editor dengan HTML dan java script
---

 Cara Memasukkan Teks Editor di HTML dengan Javascript
>Teks Editor merupakan sebuah form khusus yang memiliki fitur-fitur seperti membuat sebuah teks menjadi bold, italic, underline, dan lain-lain, secara sederhananya, ketika kamu membuat sebuah artikel baru di blogspot / wordpress, terdapat sebuah form khusus untuk menempatkan isi artikelnya, form itu merupakan sebuah Teks Editor.
>
## kode lengkap 
<script src="https://gist.github.com/MadeWiguna/a779a6965a5ad2857d710ab03b049508.js"></script>

## Demo

  
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>Summernote</title>
    <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/summernote/0.8.11/summernote-lite.css" rel="stylesheet">
    <script src="https://cdnjs.cloudflare.com/ajax/libs/summernote/0.8.11/summernote-lite.js"></script>
  </head>
  <body>
    <div id="summernote"></div>
    <script>
      $('#summernote').summernote({
        placeholder: 'Made wiguna project',
        tabsize: 2,
        height: 100
      });
    </script>
  </body>
</html> 
 

