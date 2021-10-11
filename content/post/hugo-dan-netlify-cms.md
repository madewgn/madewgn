---
title: "Hugo Dan Netlify Cms"
date: 2021-10-02T14:13:19Z
draft: true
---

Tambahkan file CMS Netlify ke Hugo
Di Hugo, file statis yang tidak perlu diproses oleh perintah build tinggal di static/direktori. Anda akan menginstal admin Netlify CMS dan file konfigurasi di sana. Buat direktori admin/dan di dalamnya, buat dua file index.htmldan config.yml. Di index.html, tambahkan konten berikut

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Content Manager</title>
    <!-- Include the script that enables Netlify Identity on this page. -->
    <script src="https://identity.netlify.com/v1/netlify-identity-widget.js"></script>
  </head>
  <body>
    <!-- Include the script that builds the page and powers Netlify CMS -->
    <script src="https://unpkg.com/netlify-cms@^2.0.0/dist/netlify-cms.js"></script>
  </body>
</html>
```

Dalam file ```config.yml```, Anda dapat menambahkan konfigurasi dasar ini - Anda dapat menyesuaikan sesuai dengan yang Anda inginkan, file sampel ini hanya untuk memulai.

```
backend:
  name: git-gateway
  branch: main # Branch to update (optional; defaults to master)
media_folder: static/img
public_folder: /img
collections:
  - name: 'blog'
    label: 'Blog'
    folder: 'content/blog'
    create: true
    slug: '{{year}}-{{month}}-{{day}}-{{slug}}'
    editor:
      preview: false
    fields:
      - { label: 'Title', name: 'title', widget: 'string' }
      - { label: 'Publish Date', name: 'date', widget: 'datetime' }
      - { label: 'Description', name: 'description', widget: 'string' }
      - { label: 'Body', name:
```
