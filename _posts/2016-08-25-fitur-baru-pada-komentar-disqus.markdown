---
layout: post
title: "Fitur Baru Pada Komentar Disqus"
subtitle: "Disqus menambahkan beberapa fitur baru pada sistem komentarnya."
description: "Disqus menambahkan beberapa fitur baru pada sistem komentarnya untuk mempermudah pengguna dalam memperjelas komentarnya."
date: 2016-08-25
author: "Adhy Suryadi"
tags: [ Blogging ]
header-img: "img/post/disqus-new-fitur.jpg"
image: "img/post/disqus-new-fitur.jpg"
---

Baru-baru ini Disqus telah menambahkan beberapa fitur baru pada sistem komentarnya untuk semakin memudahkan penggunanya untuk lebih akraktif dalam menulis komentarnya.

Beberapa fitur Disqus yang telah ada sebelumnya diantaranya pada komentar Disqus bisa menggunakan `<strong></strong>`, `<b></b>`, `<em></em>`, `<i></i>`, `<u></u>`, `<strike></strike>`, `<code></code>`, `<pre></pre>`, `<pre><code></code></pre>` untuk beberapa penulisan dalam kolom komentar. Fitur lainnya yaitu upload image dan menampilkan iframe video, mengedit komentar sendiri, atau membagikan komentar ke sosial media seperti Twitter, Facebook, ataupun lainnya.

Dan fitur baru yang telah ditambahkan yaitu memungkinkan pengguna untuk menggunakan tag `<spoiler></spoiler>` untuk show hide konten komentar pada hover. Fitur lainnya yaitu meningkatkan deteksi spam komentar menjadi lebih baik, dan juga kini kita bisa embed komentar pada postingan blog seperti di bawah ini.

<script>
document.write('<iframe src="https://embed.disqus.com/p/1b8lq6n" width="420" height="300" seamless="seamless" scrolling="no" frameborder="0" allowtransparency="true"></iframe>');
</script>

Kode embed di atas dihasilkan dari kode di bawah ini.

```html
<iframe src="https://embed.disqus.com/p/1b8lq6n" width="420" height="300" seamless="seamless" scrolling="no" frameborder="0" allowtransparency="true"></iframe>
```

Atau bisa seperti di bawah ini.

```html
<script>
document.write('<iframe src="https://embed.disqus.com/p/1b8lq6n" width="420" height="300" seamless="seamless" scrolling="no" frameborder="0" allowtransparency="true"></iframe>');
</script>
```

Untuk mendapatkan kode embed iframe ini, silahkan hover tombol **Share** pada bagian bawah komentar yang ingin dibuat embed lalu copy **link** yang muncul.

Setelah meng-copy link komentar, silahkan masuk **[di sini](https://embed.disqus.com/ "Embed Disqus Comments"){: target="_blank" rel="nofollow"}** lalu paste-kan link-nya pada kotak yang disediakan dan copy kode embed iframe yang dihasilkan.

Jika embed iframenya ingin menjadi responsive, bisa menggunakan kode di bawah ini.

```html
<script>
document.write('<div style="text-align:center;margin:0 auto;width:100%;"><div style="position:relative;padding-bottom:56.25%;height:0;overflow:hidden;margin:0;"><iframe src="LINK EMBED IFRAME DISQUS DI SINI" style="border:0;position:absolute;top:0;left:0;width:100%;height:100%;" allowfullscreen></iframe></div></div>');
</script>
```

Dan akan tampil seperti di bawah ini.

<script>
document.write('<div style="text-align:center;margin:0 auto;width:100%;"><div style="position:relative;padding-bottom:56.25%;height:0;overflow:hidden;margin:0;"><iframe src="https://embed.disqus.com/p/1b8lq6n" style="border:0;position:absolute;top:0;left:0;width:100%;height:100%;" allowfullscreen></iframe></div></div>');
</script>

Namun sayang, untuk fitur Reveal atau monitize pada Disqus sampai saat ini masih belum bisa untuk blog berbahasa Indonesia. Mudah-mudahan ke depannya reveal Disqus bisa untuk blog Indonesia.
