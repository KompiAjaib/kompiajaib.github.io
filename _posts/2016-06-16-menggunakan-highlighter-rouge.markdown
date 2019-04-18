---
layout: post
title: "Menggunakan Syntax Highlighter Rouge Di Github Pages"
subtitle: "Highlighter Rouge Mendukung 60 Bahasa Pemograman"
description: "Mencoba menggunakan syntax highlighter Rouge sebagai highlighter bawaan Jekyll."
date: 2016-06-16
author: "Adhy Suryadi"
tags: [ GithubPages, Markdown ]
header-img: "img/post/higlighter.jpg"
image: "img/post/higlighter.jpg"
social-js: "https://cdn.ampproject.org/v0/amp-social-share-0.1.js"
iframe-js: "https://cdn.ampproject.org/v0/amp-iframe-0.1.js"
accordion-js: "https://cdn.ampproject.org/v0/amp-accordion-0.1.js"
---

Sebelumnya saya memposting cara mudah menggunakan syntax highlighter dengan **[Highlight.js](http://adhysuryadi.xyz/memasang-highlight-di-github-pages/ "Highlight.js"){: target="_blank"}**. Namun kini kita akan mencoba menggunakan highlighter bawaan Jekyll yaitu **Rouge**.

Secara default, Jekyll sudah dilengkapi dengan syntax highlighter untuk mempercantik tampilan kode di blog dengan **Rouge** yang mendukung sekitar 60 bahasa pemograman. Jadi untuk memeriksa apakah theme Jekyll yang Anda gunakan telah dilengkapi *highlighter Rouge* silahkan cek di **_config.tml**, pastikan di situ terdapat `highlighter: rouge`

Namun berbeda dengan Highlight.js yang dapat secara otomatis mengenali bahasa kode, dengan Rouge kita harus menuliskan bahasa kode setiap kali kita menuliskan kode di postingan seperti `css`, `html`, `javascript`, dan lainnya sesuai dengan kode yang kita tulis.
{% include adsense_middle_post.html %}
Pada markdown, untuk menampilkan highlighter Rouge ini bisa ditulis seperti ini

```html
 ```css
 body {
  font-family: 'Lora', 'Times New Roman', serif;
  font-size: 20px;
  color: #404040;
  top:0!important
 }
 ```
```

Akan tampak seperti di bawah ini

```css
 body {
  font-family: 'Lora', 'Times New Roman', serif;
  font-size: 20px;
  color: #404040;
  top:0!important
 }
```

Atau untuk javascript seperti di bawah ini

```html
 ```javascript
 var s = "JavaScript syntax highlighting";
 alert(s);
 ```
```

Akan tampak seperti di bawah ini

```javascript
 var s = "JavaScript syntax highlighting";
 alert(s);
```

Mudah bukan? Untuk tanda seperti titik tiga (```) itu menggunakan tombol di pojok kiri atas keyboard di bawah tombol <kbd>Esc</kbd> seperti pada gambar di bawah ini.

<amp-img src="{{ site.baseurl }}/img/post/kbkoreanblack.jpg"
      width="614"
      height="388"
      layout="responsive"
      alt="Keyboard"></amp-img>

Jika Anda ingin mengganti theme untuk highlighter, Anda bisa memilih dan menggunakan css theme Pygments **[DI SINI](http://jwarby.github.io/jekyll-pygments-themes/languages/javascript.html "Pygments Themes"){: target="_blank"}** seperti pada blog ini menggunakan theme *Monokai*.
