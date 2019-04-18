---
layout: post
title: "Memasang Highlight.js Di Github Pages"
subtitle: "Mempercantik tampilan pre tags di postingan dengan syntax highlighter Highlight.js"
description: "Untuk mempercantik tampilan pre tags di postingan, bisa menggunakan syntax highlighter highlight.js yang dapat membaca semua bahasa kode."
date: 2016-06-03
author: "Adhy Suryadi"
tags: [ GithubPages ]
header-img: "img/post/highlight.jpg"
image: "img/post/highlight.jpg"
social-js: "https://cdn.ampproject.org/v0/amp-social-share-0.1.js"
iframe-js: "https://cdn.ampproject.org/v0/amp-iframe-0.1.js"
accordion-js: "https://cdn.ampproject.org/v0/amp-accordion-0.1.js"
---

Jika blog Anda membahas tentang tutorial kode, maka dipastikan Anda akan menampilkan kode-kode di postingan. Biasanya untuk menampilkan kode di postingan akan mengunakan tag pre.

Nah untuk mempercantik tampilan kode dengan tag pre, maka salah satu syntax highlighter yang saya rekomendasikan adalah highlight.js karena selain mudah dalam memasangnya juga highlight.js akan otomatis membaca bahasa kode seperti yang saya gunakan pada blog ini.

Jika Anda tertarik untuk mencobanya juga, silahkan ikuti langkah-langkahnya di bawah ini.

Silahkan buat file baru `highlight.js` di repo blog Anda di folder **js** dan silahkan copy kode dari **[sini](https://github.com/KompiAjaib/public/blob/master/highlight.js "Kode js highlight.js"){: target="_blank"}**.
{% include adsense_middle_post.html %}
Kemudian silahkan tambahkan CSS highlight.js pada CSS blog Anda di folder **css** dan silahkan copy kode dari **[sini](https://github.com/KompiAjaib/public/blob/master/highlight.css "Kode css highlight.js"){: target="_blank"}** atau untuk menggunakan style lainnya silahkan pilih css style dari **[sini](https://highlightjs.org/static/demo/ "Kode css highlight.js"){: target="_blank"}**.

Sekarang yang terakhir silahkan buka **_includes** >> **footer.html** dan simpan kode di bawah ini di bagian paling bawah.

```html
<script>
function downloadJSAtOnload() {
var element = document.createElement("script");
element.src = "{{ "/js/highlight.js " | prepend: site.baseurl }}";
document.body.appendChild(element);
}
if (window.addEventListener)
window.addEventListener("load", downloadJSAtOnload, false);
else if (window.attachEvent)
window.attachEvent("onload", downloadJSAtOnload);
else window.onload = downloadJSAtOnload;
</script>
```

Pada tutorial ini, kita men-_defer_ file js dari highlight.js agar tidak terdeteksi blocking render js.

Selamat mencoba.
