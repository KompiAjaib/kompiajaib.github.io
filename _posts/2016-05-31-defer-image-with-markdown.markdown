---
layout: post
title: "Memasangkan Dimension Tags Dan Defer Image Post Di Github Pages"
subtitle: "Cara menampilkan image dengan dimension tag dan defer pada markdown Github Pages."
description: "Cara menampilkan image dengan dimension tag dan defer pada markdown untuk optimasi blog di Github Pages."
date: 2016-05-31
author: "Adhy Suryadi"
tags: [ Markdown ]
header-img: "img/post/image-on-markdown.jpg"
image: "img/post/image-on-markdown.jpg"
social-js: "https://cdn.ampproject.org/v0/amp-social-share-0.1.js"
iframe-js: "https://cdn.ampproject.org/v0/amp-iframe-0.1.js"
accordion-js: "https://cdn.ampproject.org/v0/amp-accordion-0.1.js"
---

Dimensi pada gambar postingan (width dan height tag) merupakan salah satu unsur untuk optimasi gambar postingan selain alt tag. Begitu pun untuk gambar postingan blog di Github Pages yang menggunakan markdown dalam menulis postingannya. Sementara defer image berfungsi untuk optimasi loading blog.

Berbeda dengan penulisan markup html image (yang sebenarnya bisa juga digunakan pada markdown) yang seperti biasa menggunakan tag `<img alt="alt text" src="url image">`, penulisan atau cara menampilkan image dengan markdown berbeda dengan markup html biasa seperti di bawah ini.

{% highlight markdown %}
![alt text](url image)
{% endhighlight %}

Jika ingin menambahkan title tag maka penulisannya seperti di bawah ini.

```markdown
![alt text](url image "title text")
```

Setidaknya itu yang ada di dalam panduan penulisan markdown untuk image.
{% include adsense_middle_post.html %}
## Menambahkan Width, Height, Dan Defer Pada Image

Untuk menambahkan `width`, `height` pada image dengan penulisan markdown maka silahkan tulis seperti di bawah ini.

```markdown
![alt text](url image "title text"){: width="" height=""}
```

Silahkan isi tanda kutip pada `width` dan `height` dengan lebar dan tinggi gambar. Nah, untuk menerapkan defer pada image silahkan tulis seperti di bawah ini.

```markdown
![alt text](data:image/png;base64,R0lGODlhAQABAAD/ACwAAAAAAQABAAACADs= "title text"){: data-src="url image" width="" height=""}
```

Kemudian silahkan simpan javascript di bawah ini di atas kode `</body>` ( **_includes** >> **footer.html** simpan paling bawah ) atau silahkan satukan dengan js theme blog Anda.

```javascript
function init() {
var imgDefer = document.getElementsByTagName('img');
for (var i=0; i<imgDefer.length; i++) {
if(imgDefer[i].getAttribute('data-src')) {
imgDefer[i].setAttribute('src',imgDefer[i].getAttribute('data-src'));
} } }
window.onload = init;
```

Untuk demonya silahkan lihat halaman berikut, [DEMO](http://adhysuryadi.xyz/perangkap-iklan/ "Demo").
