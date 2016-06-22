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
---

Ketika pertama mengenal blog dengan Github Pages, saya sempat kebingungan cara menulis postingan blog karena editor ang berbeda dengan Blogger maupun Wordpress yang sudah saya kenal terlebih dahulu.

Ditambah lagi pada editor markdown Github Pages ini tidak ada tombol untuk menyimpan hasil tulisan sebagai draft postingan terlebih dahulu, alhasil selama ini saya menulis satu postingan langsung selesai dan langsung dipublikasikan.

Pernah pada suatu waktu telah menulis postingan panjang lebar, dan kesalahan pencet tombol me-reload halaman editor postingan sehingga tulisan yang sudah panjang lebih jadi hilang tanpa tersimpan di draft postingan. Nyesel banget kan hik...hik...hik...

Itulah pengalaman menggelikan menulis postingan di Github Pages karena keterbatasan pengetahuan hehehe... namun akhirnya jadi pengalaman berharga yang kini bisa saya bagikan pengalaman ini kepada Anda.

Sebenarnya Github Pages mendukung penulisan postingan draft, artinya kita bisa menyimpan tulisan terlebih dahulu dan kemudian melanjutkan atau mempublikasikan tulisannya di hari yang lain.

Pada Jekyll, draft postingan adalah postingan yang ditulis tanpa format tanggal pada URL postingan.

Seperti kita ketahui, untuk menerbitkan postingan kita harus membuat postingan dengan URL seperti berikut:

```markdown
YYYY-MM-DD-title.markdown
```

Jika kita membuat URL postingan tanpa `YYYY-MM-DD` maka postingan tidak bisa dipublikasikan.

Nah untuk membuat draft postingan, silahkan menuju repository blog Anda dan buat file baru dengan nama file **_draft/draft-postingan.markdown** kemudian **Commit** file tersebut.

Dengan itu kita berhasil membuat sebuah folder **_draft** dengan isinya file **draft-postingan.markdown**. Untuk mulai menulis draft postingan silahkan edit file **draft-postingan.markdown** tersebut. Kemudian jika mau berhenti menulis, Anda tinggal **Commit** tulisan. Dan jika ingin melanjutkan tulisan tinggal edit saja filenya.

