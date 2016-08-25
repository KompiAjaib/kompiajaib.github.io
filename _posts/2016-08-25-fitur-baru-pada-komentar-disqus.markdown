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

Beberapa fitur Disqus yang telah ada sebelumnya diantaranya pada komentar Disqus bisa menggunakan `&lt;strong&gt;&lt;/strong&gt;`, `&lt;b&gt;&lt;/b&gt;`, `&lt;em&gt;&lt;/em&gt;`, `&lt;i&gt;&lt;/i&gt;`, `&lt;u&gt;&lt;/u&gt;`, `&lt;strike&gt;&lt;/strike&gt;`, `&lt;code&gt;&lt;/code&gt;`, `&lt;pre&gt;&lt;/pre&gt;`, `&lt;pre&gt;&lt;code&gt;&lt;/code&gt;&lt;/pre&gt;` untuk beberapa penulisan dalam kolom komentar. Fitur lainnya yaitu upload image dan menampilkan iframe video, mengedit komentar sendiri, atau membagikan komentar ke sosial media seperti Twitter, Facebook, ataupun lainnya.

Dan fitur baru yang telah ditambahkan yaitu memungkinkan pengguna untuk menggunakan tag `&lt;spoiler&gt;&lt;/spoiler&gt;` untuk show hide konten komentar pada hover. Fitur lainnya yaitu meningkatkan deteksi spam komentar menjadi lebih baik, dan juga kini kita bisa embed komentar pada postingan blog seperti di bawah ini.

<script>
//<![CDATA[
document.write('<iframe data-src="https://embed.disqus.com/p/1b8lq6n" width="420" height="300" seamless="seamless" scrolling="no" frameborder="0" allowtransparency="true"></iframe>');
//]]>
</script>

Kode embed di atas dihasilkan dari kode di bawah ini.

```
&lt;iframe src="https://embed.disqus.com/p/1b8lq6n" width="420" height="300" seamless="seamless" scrolling="no" frameborder="0" allowtransparency="true"&gt;&lt;/iframe&gt;
```

Atau bisa seperti di bawah ini.

```
&lt;script&gt;<br />
//&lt;![CDATA[<br />
document.write('&lt;iframe src="https://embed.disqus.com/p/1b8lq6n" width="420" height="300" seamless="seamless" scrolling="no" frameborder="0" allowtransparency="true"&gt;&lt;/iframe&gt;');<br />
//]]&gt;<br />
&lt;/script&gt;
```

Untuk mendapatkan kode embed iframe ini, silahkan hover tombol **Share** pada bagian bawah komentar yang ingin dibuat embed lalu copy link yang muncul.

Setelah meng-copy link komentar, silahkan masuk **[di sini](https://embed.disqus.com/ "Embed Disqus Comments"){: target="_blank" rel="nofollow"}** lalu paste-kan link-nya pada kotak yang disediakan dan copy kode embed iframe yang dihasilkan.

Jika embed iframenya ingin menjadi responsive, bisa menggunakan kode di bawah ini.

```
&lt;script&gt;<br />
//&lt;![CDATA[<br />
document.write('&lt;div style="text-align:center;margin:0 auto;width:100%;"&gt;&lt;div style="position:relative;padding-bottom:56.25%;height:0;overflow:hidden;margin:0;"&gt;&lt;iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3953.9207513330716!2d108.6513236!3d-7.6916542!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0xf18aa9a899b3191e!2sPondok+Nankenz!5e0!3m2!1sen!2s!4v1441874163329" style="border:0;position:absolute;top:0;left:0;width:100%;height:100%;" allowfullscreen&gt;&lt;/iframe&gt;&lt;/div&gt;&lt;/div&gt;');<br />
//]]&gt;<br />
&lt;/script&gt;
```

Dan akan tampil seperti di bawah ini.

<script>
//<![CDATA[
document.write('<div style="text-align:center;margin:0 auto;width:100%;"><div style="position:relative;padding-bottom:56.25%;height:0;overflow:hidden;margin:0;"><iframe data-src="https://embed.disqus.com/p/1b8lq6n" style="border:0;position:absolute;top:0;left:0;width:100%;height:100%;" allowfullscreen></iframe></div></div>');
//]]>
</script>

Namun sayang, untuk fitur Reveal atau monitize pada Disqus sampai saat ini masih belum bisa untuk blog berbahasa Indonesia. Mudah-mudahan ke depannya reveal Disqus bisa untuk blog Indonesia.
