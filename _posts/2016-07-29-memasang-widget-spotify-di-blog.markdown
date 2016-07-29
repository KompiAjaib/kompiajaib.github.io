---
layout: post
title: "Memasang Widget Spotify Di Blog"
subtitle: "Menampilkan lagu-lagu favorite dari Spotify di blog."
description: "Menampilkan lagu-lagu favorite dari Spotify di blog untuk dinikmati juga oleh orang lain."
date: 2016-07-29
author: "Adhy Suryadi"
tags: [ Blogging ]
header-img: "img/post/spitify.jpg"
image: "img/post/spitify.jpg"
---

Seperti kita ketahui bahwa Spotify merupakan sebuah aplikasi yang menyediakan jutaan lagi-lagu pilihan dari seluruh dunia. Jadi tidak akan rugi jika kita menginstall aplikasi Spotify ini di komputer, laptop, atau bahkan di smartphone kita.

Jutaan lagu mulai dari lagu-lagu lawas, lagu-lagu daerah/tradisional, lagu pop, rock, jazz, lagu yang lagi hit, bahkan lagu yang baru dirilis tersedia di Spotify.

Selain menginstall aplikasi di perangkat kita, kita juga bisa menampilkan lagu-lagu favorite kita di blog untuk dinikmati juga oleh orang lain.

Bisa berupa single song maupun play list yang ditampilkan di blog. Untuk menampilkan widget Spotify di blog cukup mudah karena kode iframe sudah disediakan oleh Spotify. Kita tinggal pilih lagu atau play list yang ingin di tampilkan kemudian copy kode embed-nya seperti pada animasi di bawah ini.

![spotify](data:image/png;base64,R0lGODlhAQABAAD/ACwAAAAAAQABAAACADs= "Copy code embed Spotify"){: data-src="https://lh4.googleusercontent.com/-cvXF8u3FscI/V5stuIPs2dI/AAAAAAAAnWw/zsQWN8pPq9c_sePzBp7cJLmJHJttJRIjgCL0B/w750-h428-no/Animation.gif" width="750" height="428"}

Setelah meng-copy kode embed-nya, silahkan paste kode tersebut pada editor HTML, biasanya kode embed-nya berupa iframe seperti di bawah ini.

```
<iframe src="https://embed.spotify.com/?uri=spotify%3Auser%3Aspotifyindonesia%3Aplaylist%3A0uyWN9oNJcc81mymCfNKP4" width="300" height="380" frameborder="0" allowtransparency="true"></iframe>
```

Jika ingin responsive, silahkan coba dengan kode di bawah ini.

```
<script>
//<![CDATA[
document.write('<div style="text-align:center;margin:0 auto;width:100%;"><div style="position:relative;padding-bottom:56.25%;height:0;overflow:hidden;margin:0;"><iframe src="https://embed.spotify.com/?uri=spotify%3Auser%3Aspotifyindonesia%3Aplaylist%3A0uyWN9oNJcc81mymCfNKP4" style="border:0;position:absolute;top:0;left:0;width:100%;height:100%;" allowfullscreen></iframe></div></div>');
//]]>
</script>
```

Dan hasilnya akan tampak seperti di bawah ini.

<script>
//<![CDATA[
document.write('<div style="text-align:center;margin:0 auto;width:100%;"><div style="position:relative;padding-bottom:56.25%;height:0;overflow:hidden;margin:0;"><iframe data-src="https://embed.spotify.com/?uri=spotify%3Auser%3Aspotifyindonesia%3Aplaylist%3A0uyWN9oNJcc81mymCfNKP4" style="border:0;position:absolute;top:0;left:0;width:100%;height:100%;" allowfullscreen></iframe></div></div>');
//]]>
</script>

Dan untuk para pengunjung blog yang ingin menikmati lagu-lagu dari Spotify yang kita tampilkan di blog, mereka juga harus meng-install aplikasi Spotify pada perangkat mereka.

Untuk men-download aplikasi Spotify, silahkan klik [di sini](https://www.spotify.com/ "download aplikasi Spotify"){: target="_blank" rel="nofollow"} dan silahkan pilih gratis atau premium.
