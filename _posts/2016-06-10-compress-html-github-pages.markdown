---
layout: post
title: "Cara Compress HTML Jekyll Blog Github Pages"
subtitle: "Membuat blog Jekyll Anda menjadi lebih cepat dimuat."
description: "Dengan compress HTML maka blog lebih cepat dan lebih optimal dalam pemuatan kode blog."
date: 2016-06-10
author: "Adhy Suryadi"
tags: [ GithubPages ]
header-img: "img/post/compress.jpg"
image: "img/post/compress.jpg"
social-js: "https://cdn.ampproject.org/v0/amp-social-share-0.1.js"
iframe-js: "https://cdn.ampproject.org/v0/amp-iframe-0.1.js"
accordion-js: "https://cdn.ampproject.org/v0/amp-accordion-0.1.js"
---

Salah satu cara untuk mempercepat dan mengotimalkan loading blog adalah dengan compress HTML. Meng-compress HTML itu diantaranya menghapus spasi yang tidak perlu, menghapus tag akhir atau start tag yang tidak perlu atau menghapus komentar yang tidak perlu dari kode HTML.

## Compress HTML Jekyll Blog

Nah, untuk blog Jekyll di Github Pages kita bisa melakukan compress HTML dengan langkah-langkah di bawah ini.

### Langkah Pertama

Silahkan download `compress.html` versi terbaru dari **[sini](https://github.com/penibelst/jekyll-compress-html/releases/ "Download"){: target="_blank" rel="nofollow"}**. Kemudian unzip file `compress.html` yang Anda download tadi.
{% include adsense_middle_post.html %}
### Langkah Kedua

Silahkan upload file `compress.html` di bagian **_layouts** dan masih di **_layouts** silahkan edit file `default.html` kemudian tambahkan kode YAML di bawah ini di paling atas

```markdown
---
layout: compress
---
```

### Langkah Ketiga

Silahkan edit file **_config.yml** dan masukan kode di bawah ini

```markdown
# html minify
compress_html:
  clippings: all
  comments: all
  endings: []
  profile: false
```

Jika Anda menggunakan kode **[perangkap iklan](http://kompiajaib.github.io/perangkap-iklan/ "perangkap iklan"){: target="_blank"}** silahkan tambahkan kode di bawah ini

```markdown
  ignore:
  comments: ["<!--</body>-->"]
```

Sehingga menjadi seperti di bawwah ini

```markdown
# html minify
compress_html:
  clippings: all
  comments: all
  endings: []
  profile: false
  ignore:
  comments: ["<!--</body>-->"]
```

Selesai, sekarang silahkan cek source code blog Anda.
