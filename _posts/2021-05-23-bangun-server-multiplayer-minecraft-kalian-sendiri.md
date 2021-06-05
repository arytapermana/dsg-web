---
title: Bangun Server Multiplayer Minecraft Kalian Sendiri
date: 2021-05-23 19:31:55 +08:00
categories:
- Info
tags:
- Ngrok
- Multiplayer
- Minecraft
layout: post
author: sal
image: https://ik.imagekit.io/dsg/thumb_RSrSNhvh5.jpg
tldr: https://disekitargame.com/stories/2021-05-23-bangun-server-multiplayer-minecraft-kalian-sendiri/
---

Minecraft ketika Bermain bersama teman terkadang cukup sulit untuk video game satu ini, kalian perlu mencari server publik ataupun membeli server premium dari Minecraft yang biasa di sebut Minecraft Realms, walaupun hanya ingin bermain bersama teman kalian, hal ini terasa cukup susah.

Teman kalian dan kalian sebenernya ketika berada pada satu jaringan yang sama kalian dapat membuat server sendiri dan membagikan ip serta port yang ada ke teman kalian, cukup mudah bukan, tapi bagaimana jika teman kalian berada di wilayah yang cukup jauh, maka jaringan internet diperlukan dan hal ini memerlukan sesuatu yang disebut port forward, yaitu membagikan alamat ip lokal yang ada untuk dapat diakses hingga ke internet. Jadi hal tersebut yang akan dibahas kali ini.

Masalah yang terkadang muncul ketika melakukan port forward sebuah jaringan adalah ISP (Internet Service Provider) yang tidak memberikan ip publik kepada pelanggan sehingga port yang akan dilakukan port forward ter-blok di sistem mereka, hanya port yang mereka ijinkan saja dapat diakses, selain itu jika kalian melakukan port forward maka ip publik kalian akan ter-expose ke jaringan internet dengan port yang terbuka, dan ini cukup berbahaya dimana dapat menjadi peluang bagi seseorang yang tidak bertanggung jawab mengakses port terbuka tersebut sehingga memberik akses ke perangkat kalian, maka dari itu kami menggunakan Ngrok, sebuah tools seperti VPN yang mengirim data kalian pada sebuah tunnel yang lebih aman, dan mengakses nya melalui url dan port berbeda yang diberikan mereka nantinya.

> Perlu diingat tutorial ini hanya bekerja untuk Minecraft versi Java, Minecraft Bedrock (cnth. Windows 10 atau Android) tidak bekerja karena menggunakan Ngrok yang akan meneruskan jaringan lokal menuju TCP yang tidak di support Minecraft Bedrock yang menggunakan UDP.

Membangun sebuah server berbeda dengan membagikan world minecraft kalian dengan teman untuk join, karena minecraft server lebih fleksibel dan customize able, jadi berikut beberapa hal yang perlu dipersiapkan terlebih dahulu sebelum memulai.

* Unduh Minecraft server pada situs resminya [disini](https://www.minecraft.net/en-us/download/server).
* Daftar akun Ngrok [disini](https://ngrok.com/).

> Pastikan versi minecraft kalian sama dengan versi server minecraft agar berjalan dengan baik.

Jika sudah maka langkah pertama adalah dengan extract file Minecraft server yang kalian unduh sebelumnya dan taruh pada direktori yang kalian inginkan atau mudah ditemukan. akses folder tersebut melalui CMD jika dari Windows dan start server Minecraft, commandnya kurang lebih sebagai berikut.

    java -jar server.jar --world m-server

[![inecraft server](https://ik.imagekit.io/dsg/m-server_aAVedRiqJ.png)](https://ik.imagekit.io/dsg/m-server_aAVedRiqJ.png){: .glightbox}


setelah memulai server maka pada log command line kalian akan melihat port yang digunakan oleh server, simpan port tersebut yang nantinya akan digunakan pada Ngrok.

[![port minecraft](https://ik.imagekit.io/dsg/m-server-1_xmoCcluHo.png)](https://ik.imagekit.io/dsg/m-server-1_xmoCcluHo.png){: .glightbox}

Setelah itu maka login pada akun Ngrok dan pada halaman awal akan disediakan pilihan mengunduhnya, lanjutkan tahapan hingga tahap dua saja yaitu sampai pada proeses menghubungkan akun.

aktifkan port forward lokal menuju server Ngrok dengan command berikut.

    ngrok tcp -region ap 25565

[![ngrok server start](https://ik.imagekit.io/dsg/m-server-2_1vxepPxJG.png)](https://ik.imagekit.io/dsg/m-server-2_1vxepPxJG.png){: .glightbox}

Setelah itu maka copy bagian alamat tcp saja tanpa menyertakan tcp, seperti berikut.

    0.tcp.ap.ngrok.io:13129

Simpan alamat ip tersebut kemudian masukan pada menu server di minecraft, saya sarankan kalian hanya menggunakan direct connection atau sekali konek karena Ngrok selalu mengubah alamat ataupun port yang digunakan setiap kali melakukan start server.

![minecraft direct connection](https://ik.imagekit.io/dsg/m-server-3_hQYpbxa-I.png)

alamat tersebut juga yang kalian dapat bagikan ke teman kalian sehingga mereka dapat join server yang kalian buat sendiri. 

Jika ada yang dibingungkan atau ditanyakan silahkan bertanya pada kolom komentar karena kami sangat antusias membaca komentar kalian, happy gaming!