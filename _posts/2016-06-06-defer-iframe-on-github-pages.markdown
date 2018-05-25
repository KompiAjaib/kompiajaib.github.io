---
layout: post
title: "Defer Iframe Video Youtube Pada Blog Github Pages"
subtitle: "Dengan defer iframe pada blog maka loading blog menjadi ringan."
description: "Dengan defer iframe video Youtube dimaksudkan agar loading iframe tidak mengganggu loading blog."
date: 2016-06-06
author: "Adhy Suryadi"
tags: [ GithubPages, Markdown ]
header-img: "img/post/defer-iframe.jpg"
image: "img/post/defer-iframe.jpg"
social-js: "https://cdn.ampproject.org/v0/amp-social-share-0.1.js"
iframe-js: "https://cdn.ampproject.org/v0/amp-iframe-0.1.js"
accordion-js: "https://cdn.ampproject.org/v0/amp-accordion-0.1.js"
youtube-js: "https://cdn.ampproject.org/v0/amp-youtube-0.1.js"
---

Kadang untuk melengkapi sebuah artikel di blog, kita perlu juga memasang sebuah video. Video yang sudah familiar dipasang di blog biasanya dari video Youtube.

Namun yang jadi masalahnya adalah pemuatan video ini sangat mengganggu loading blog. Untuk itu kita perlu menunda pemuatan iframe video Youtube sehingga pemuatan elemen blog lainnya tidak terganggu, sementara iframe video Youtube akan dimuat setelah semua elemen termuat atau istilahnya "**lazy loading iframe**".

Nah untuk menunda pemuatan iframe (*defer iframe*) video Youtube di blog Github Pages ini bisa dilakukan dengan langkah seperti berikut:

Silahkan simpan kode javascript di bawah ini di atas kode `</body`, silahkan buka **_includes** >> **footer.html** dan simpan di paling bawah.

```html
<script>
function init() {
    var vidDefer = document.getElementsByTagName('iframe');
    for (var i = 0; i < vidDefer.length; i++) {
        if (vidDefer[i].getAttribute('data-src')) {
            vidDefer[i].setAttribute('src', vidDefer[i].getAttribute('data-src'));
        }
    }
}
window.onload = init;
</script>
```

Kemudian untuk menampilkan video di dalam postingan, silahkan tambahkan `data` pada `src` embed video Youtube menjadi `data-src` seperti di bawah ini:

**Kode embed awal**

```html
<iframe width="560" height="315" src="https://www.youtube.com/embed/zBASI-CQxw4" frameborder="0" allowfullscreen></iframe>
```

Menjadi seperti di bawah ini **Kode embed untuk defer iframe**

```html
<iframe width="560" height="315" data-src="https://www.youtube.com/embed/zBASI-CQxw4" frameborder="0" allowfullscreen></iframe>
```

**Live Demo**

Video di bawah ini sudah menggunakan *defer iframe* dengan kode embed di atas.

<amp-youtube width="560"
      height="315"
      layout="responsive"
      data-videoid="zBASI-CQxw4">
  </amp-youtube>
