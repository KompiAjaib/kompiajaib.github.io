---
layout: post
title: "Cara Embed Font Awesome Di Blog Berubah"
subtitle: "Semakin mudah dalam menggunakan Font Awesome dengan kode embed terbaru."
description: "Kini semakin mudah dalam menggunakan Font Awesome di blog, bahkan kini kita bisa me-manage font awesome."
date: 2016-06-07
author: "Adhy Suryadi"
tags: [ Blogging ]
header-img: "img/post/font-awesome.jpg"
image: "img/post/font-awesome.jpg"
social-js: "https://cdn.ampproject.org/v0/amp-social-share-0.1.js"
iframe-js: "https://cdn.ampproject.org/v0/amp-iframe-0.1.js"
accordion-js: "https://cdn.ampproject.org/v0/amp-accordion-0.1.js"
---

Baru hari ini saya menyadari bahwa kini cara embed Font Awesome telah berubah. Yang sangat mencolok dari perubahan ini adalah cara mendapatkan kode embed-nya, kini tidak ada lagi link CDN Font Awesome pada halaman **Get Started** Font Awesome. Namun yang ada adalah kolom input email untuk mendapatkan kode embed Font Awesome.

> We create new embed codes for each website so you can quickly upgrade and change your preferences all without ever pushing code. To do this, we need an email address so we know which embed codes are yours and so you can come back and manage them.

Itulah alasan dari Font Awesome untuk mendapatkan kode embed dengan menggunakan email.

Ternyata kini kita mendapatkan dashboard Font Awesome CDN untuk memanage Font Awesome yang kita gunakan. Di dashboard ini juga kita bisa dengan mudah mengupdate Font Awesome jika terdapat update dari Font Awesome.

Kita pun bisa memiliki kode embed Font Awesome yang berbeda untuk setiap blog yang kita miliki.
{% include adsense_middle_post.html %}
Silahkan dicoba dengan memasukan email Anda pada input email di halaman **Get Started** Font Awesome. Kemudian silahkan cek kotak masuk email Anda, maka di situ akan terdapat kode embed berupa file JS dan silahkan klik tombol **Register my Font Awesome CDN account** untuk mendapat dashboard Font Awesome CDN kita sendiri.

## Pemasangan Kode Font Awesome

Untuk pemasangan kode JS Font Awesome bisa juga dengan asynchronous untuk menghindari *blocking render js* seperti di bawah ini.

```html
<script async src="https://use.fontawesome.com/xxxxxxxxx.js"></script>
```

Atau seperti ini

```html
<script async="async" src="https://use.fontawesome.com/xxxxxxxxx.js"></script>
```

Atau seperti ini

```html
<script async="async" defer="defer" src="https://use.fontawesome.com/xxxxxxxxx.js"></script>
```

Atau menggunakan javascript dinamis asyncronous seperti Google+ JS.

```javascript
  (function() {
    var po = document.createElement('script'); po.type = 'text/javascript'; po.async = true;
    po.src = 'https://use.fontawesome.com/xxxxxxxxx.js';
    var s = document.getElementsByTagName('script')[0]; s.parentNode.insertBefore(po, s);
  })();
```

Silahkan dicoba cara embed Font Awesome terbaru ini **[DI SINI](http://fontawesome.io/get-started/ "Get Started Font Awesome"){: target="_blank" rel="nofollow"}**
