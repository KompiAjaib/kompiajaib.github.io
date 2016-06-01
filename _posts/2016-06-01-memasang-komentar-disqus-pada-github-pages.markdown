---
layout: post
title: "Memasang Komentar Disqus Pada Github Pages"
subtitle: "Cara memasang sistem komentar Disqus pada Jekyll blog di Github Pages."
description: "Sebagai web statis, blog di Github Pages memerlukan sistem komentar dari pihak ketiga seperti Disqus."
date: 2016-06-01
author: "Adhy Suryadi"
tags: [ GithubPages ]
header-img: "img/disqus.jpg"
image: "img/disqus.jpg"
---

Sebagai web statis, blog berbasis Jekyll di Github Pages tidak memiliki sistem komentar sendiri. Untuk itu dibutuhkan sistem komentar pihak ketiga seperti Disqus, Facebook, dan lainnya.

## Memasang Komentar Disqus

Nah kini kita akan memasang sistem komentar Disqus pada Jekyll blog di Github Pages. Silahkan ikuti langkah-langkahnya di bawah ini:

Silahkan buat dulu akun disqus untuk blog Anda di sini *https://disqus.com/admin/signup/*. Setelah selesai, silahkan catat username disqus blog Anda.

Kemudian silahkan buka repository blog Anda dan buat file `disqus_comments.html` pada bagian **_includes** kemudian copy kode di bawah ini lalu paste di editor markdown.

```
<div id="disqus_thread"></div>
<script>
    var disqus_config = function () {
this.page.url = "PAGE_URL"; // Replace PAGE_URL with your page's canonical URL variable
this.page.identifier = "PAGE_IDENTIFIER"; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
};
</script>
```
Ganti `PAGE_URL` dengan `page.url | replace:'index.html','' | prepend: site.baseurl | prepend: site.url` dengan tag `{{ }}`.

Ganti `PAGE_IDENTIFIER` dengan `page.url | prepend: site.baseurl` dengan tag `{{ }}`.

Kemudian bukan **_includes** >> **footer.html** lalu simpan kode di bawah ini di bagian paling bawah atau bisa disatukan dengan js theme blog Anda.

```
!function(){var e=document,t=e.createElement("script");t.src="//username.disqus.com/embed.js",t.setAttribute("data-timestamp",+new Date),(e.head||e.body).appendChild(t)}();
```

Silahkan ganti kode `username` dengan username disqus blog Anda.

Kemudian buka *_layouts* >> *post.html* lalu silahkan copy kode `include disqus_comments.html` dan silahkan simpan di bawah kode `content`.

Selesai, silahkan coba buka salah satu postingan blog Anda untuk melihat penampakan komentar Disqus.

Selamat mencoba...
