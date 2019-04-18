---
layout: post
title: "Membuat Draft Postingan Blog Di Github Pages"
subtitle: "Untuk mempermudah membuat postingan blog dengan terjadwal."
description: "Dengan menggunakan draft postingan, kita dapat membuat postingan dengan menundanya hari ini dan melanjutkannya esok hari."
date: 2016-06-22
author: "Adhy Suryadi"
tags: [ GithubPages ]
header-img: "img/post/draft.jpg"
image: "img/post/draft.jpg"
social-js: "https://cdn.ampproject.org/v0/amp-social-share-0.1.js"
iframe-js: "https://cdn.ampproject.org/v0/amp-iframe-0.1.js"
accordion-js: "https://cdn.ampproject.org/v0/amp-accordion-0.1.js"
---

Ketika pertama mengenal blog dengan Github Pages, saya sempat kebingungan cara menulis postingan blog karena editor yang berbeda dengan Blogger maupun Wordpress yang sudah saya kenal terlebih dahulu.

Ditambah lagi pada editor markdown Github Pages ini tidak ada tombol untuk menyimpan hasil tulisan sebagai draft postingan terlebih dahulu, alhasil selama ini saya menulis satu postingan langsung selesai dan langsung dipublikasikan.

Pernah pada suatu waktu telah menulis postingan panjang lebar, dan kesalahan pencet tombol me-reload halaman editor postingan sehingga tulisan yang sudah panjang lebih jadi hilang tanpa tersimpan di draft postingan. Nyesel banget kan hik...hik...hik...

Itulah pengalaman menggelikan menulis postingan di Github Pages karena keterbatasan pengetahuan hehehe... namun akhirnya jadi pengalaman berharga yang kini bisa saya bagikan pengalaman ini kepada Anda.

Sebenarnya Github Pages mendukung penulisan postingan draft, artinya kita bisa menyimpan tulisan terlebih dahulu dan kemudian melanjutkan atau mempublikasikan tulisannya di hari yang lain.
{% include adsense_middle_post.html %}
Pada Jekyll, draft postingan adalah postingan yang ditulis tanpa format tanggal pada URL postingan.

Seperti kita ketahui, untuk menerbitkan postingan kita harus membuat postingan dengan URL seperti berikut:

```markdown
YYYY-MM-DD-title.markdown
```

Jika kita membuat URL postingan tanpa `YYYY-MM-DD` maka postingan tidak bisa dipublikasikan.

Nah untuk membuat draft postingan, silahkan menuju repository blog Anda dan buat file baru dengan nama file **_drafts/draft-postingan.markdown** kemudian **Commit** file tersebut.

Dengan itu kita berhasil membuat sebuah folder **_drafts** dengan isinya file **draft-postingan.markdown**.

Untuk mulai menulis draft postingan silahkan buat file baru di dalam folder **_drafts** tersebut dengan URL postingan tanpa format tanggal seperti file yang pertama dibuat tadi. Kemudian jika mau berhenti menulis, Anda tinggal **Commit** tulisan. Dan jika ingin melanjutkan tulisan tinggal edit saja filenya.

Jika ingin mempublikasikan tulisan maka tinggal edit URL postingannya dengan menambahkan format `YYYY-MM-DD` pada URL postingan. Kemudian ganti juga **_drafts** menjadi **_posts** agar tulisan yang dipublikasikan masuk ke folder **_posts** dengan <kbd>Backspace</kbd> di depan URL postingan. Atau kalau bingung, hapus semua URL draft postingan dan tulis kembali seperti ini **_posts/2016-06-22-inilah-postingan-dari-drafts.markdown**

Sebagai contoh postingan ini saya buat dari draft postingan.

Selamat mencoba.
