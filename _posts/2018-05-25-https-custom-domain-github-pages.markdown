---
layout: post
title: "Akhirnya Custom Domain Github Pages Support HTTPS"
subtitle: "Kini custom domain di GitHub Pages mendapatkan dukungan untuk HTTPS, dan berikut cara mengaktifkannya."
description: "Saat ini, custom domain di GitHub Pages mendapatkan dukungan untuk HTTPS, yang berarti lebih dari satu juta situs GitHub Pages akan dilayani melalui HTTPS. Dan berikut cara mengaktifkan HTTPS custom domain pada Github Pages."
date: 2018-05-25
author: "Adhy Suryadi"
tags: [ GithubPages ]
header-img: "img/post/https-custom-domain.png"
image: "img/post/https-custom-domain.png"
social-js: "https://cdn.ampproject.org/v0/amp-social-share-0.1.js"
iframe-js: "https://cdn.ampproject.org/v0/amp-iframe-0.1.js"
accordion-js: "https://cdn.ampproject.org/v0/amp-accordion-0.1.js"
---

Setelah cukup lama menunggu support HTTPS untuk custom domain pada Github Pages, akhirnya kini custom domain di GitHub Pages mendapatkan dukungan untuk HTTPS. Ini berarti lebih dari satu juta situs GitHub Pages akan dilayani melalui HTTPS.

Hal ini tentunya merupakan kabar baik bagi pengguna Github Pages, bahwa kini situs memberikan lalu lintas yang aman. Seperti kita tahu bahwa HTTPS (dikenal dengan ikon kunci hijau di bilah alamat browser) mengenkripsi lalu lintas antara server GitHub dan browser. Ini memberikan keyakinan kepada pengunjung bahwa halaman situs yang mereka kunjungi benar-benar halaman yang ingin mereka kunjungi.

Apalagi ke depannya, khususnya browser Google Chrome akan memberikan peringatan **tidak aman** pada situs yang masih menggunakan HTTP pada address bar browser.
{% include adsense_middle_post.html %}
Jika Anda penggunakan Github Pages dan menggunakan custom domain pada blognya, silahkan segera aktifkan HTTPS untuk custom domain blog Anda. HTTPS ini diberian gratis untuk semua pengguna Github Pages.

Cara mengaktifkannya juga cukup mudah, Anda tinggal mengganti **IP address** pada setting DNS domain Anda. Silahkan ganti IP address pada setting DNS domain Anda dengan IP address berikut.

```html
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

Setelah mengganti IP Address, silahkan tunggu sekitar 12 - 24 jam untuk waktu propagasi. Setelah itu silahkan masuk ke repository blog Anda lalu klik menu **Setting** di kanan atas, lalu pada bagian custom domain silahkan hapus domain blog Anda lalu **Save**.

Silahkan refresh halaman **Setting** tadi lalu silahkan pasang kembali domainnya dan **Save**. Kemudian refresh lagi dan cek bagian **Enforce HTTPS** di bawah domain. Jika sudah available silahkan centang **Enforce HTTPS** untuk mengaktifkan HTTPS. Jika belum memungkinkan maka Anda harus menunggu lagi dan kemudian ulangi lagi dengan mencopot domain Anda sampai bisa mencentang **Enforce HTTPS**.

Bagaimana, mudah bukan?

Happy blogging...
