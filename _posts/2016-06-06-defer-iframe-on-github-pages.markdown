---
layout: post
title: "Defer Iframe Video Youtube Pada Blog Github Pages"
subtitle: "Dengan defer iframe pada blog agar loading blog menjadi ringan."
description: "Dengan defer iframe video Youtube dimaksudkan agar loading iframe tidak mengganggu loading blog."
date: 2016-06-06
author: "Adhy Suryadi"
tags: [ GithubPages, Markdown ]
header-img: "img/post/defer-iframe.jpg"
image: "img/post/defer-iframe.jpg"
---

Kadang untuk melengkapi sebuah artikel di blog, kita perlu juga memasang sebuah video. Video yang sudah familiar dipasang di blog biasanya dari video Youtube.

Namun yang jadi masalahnya adalah pemuatan video ini sangat mengganggu loading blog. Untuk itu kita perlu menunda pemuatan iframe video Youtube sehingga pemuatan elemen blog lainnya tidak terganggu, sementara iframe video Youtube akan dimuat setelah semua elemen termuat atau istilahnya "**lazy loading iframe**".

Nah untuk menunda pemuatan iframe (*defer iframe*) video Youtube di blog Github Pages ini bisa dilakukan dengan langkah seperti berikut:

Silahkan simpan kode javascript di bawah ini di atas kode `</body`, silahkan buka **_includes** >> **footer.html** dan simpan di paling bawah.

```
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

```
<iframe width="560" height="315" data-src="https://www.youtube.com/embed/zBASI-CQxw4" frameborder="0" allowfullscreen></iframe>
```

**Live Demo**

Video di bawah ini sudah menggunakan *defer iframe* seperti di atas.

<iframe width="560" height="315" data-src="https://www.youtube.com/embed/zBASI-CQxw4" frameborder="0" allowfullscreen></iframe>
