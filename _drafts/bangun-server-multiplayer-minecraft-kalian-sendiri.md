---
layout: post
author: sal
date: 2021-05-23 19:31:55 +0800
title: Bangun Server Multiplayer Minecraft Anda Sendiri
categories:
- Info
tags:
- Ngrok
- Multiplayer
- Minecraft
image: https://ik.imagekit.io/dsg/thumb_RSrSNhvh5.jpg
tldr: ''

---
    Bermain bersama teman terkadang cukup sulit untuk video game satu ini, kalian perlu mencari server publik ataupun membeli server premium dari Minecraft itu sendiri atau biasa di sebut Minecraft Realms, walaupun hanya ingin bermain bersama teman kalian, hal ini terasa cukup susah.

sebenarnya jika kalian dan teman kalian berada pada satu jaringan yang sama kalian dapat membuat server sendiri dan membagikan ip serta port yang ada ke teman kalian, cukup mudah bukan, tapi bagaimana jika teman kalian berada di wilayah yang cukup jauh, maka jaringan internet diperlukan dan hal ini memerlukan sesuatu yang disebut port forward, yaitu membagikan alamat ip lokal yang ada untuk dapat diakses hingga ke internet. Jadi hal tersebut yang akan dibahas kali ini.

Masalah yang terkadang muncul ketika melakukan port forward sebuah jaringan adalah ISP (Internet Service Provider) yang tidak memberikan ip publik kepada pelanggan sehingga port yang akan dilakukan port forward ter-blok di sistem mereka, hanya port yang mereka ijinkan saja dapat diakses, selain itu jika kalian melakukan port forward maka ip publik kalian akan ter-expose ke jaringan internet dengan port yang terbuka, dan ini cukup berbahaya dimana dapat menjadi peluang bagi seseorang yang tidak bertanggung jawab mengakses port terbuka tersebut sehingga memberik akses ke perangkat kalian, maka dari itu kami menggunakan Ngrok yang, sebuah tools seperti VPN yang mengirim data kalian pada sebuah tunnel yang lebih aman, dan mengakses nya melalui url dan port berbeda yang diberikan mereka nantinya.

> Perlu diingat tutorial ini hanya bekerja untuk Minecraft versi Java, Minecraft Bedrock (cnth. Windows 10 atau Android) tidak bekerja karena menggunakan Ngrok yang akan meneruskan jaringan lokal menuju TCP yang tidak di support Minecraft Bedrock yang menggunakan UDP.

Membangun sebuah server berbeda dengan membagikan world minecraft kalian dengan teman untuk join, karena minecraft server lebih fleksibel dan customize able, jadi berikut beberapa hal yang perlu dipersiapkan terlebih dahulu sebelum memulai.

* Unduh Minecraft server pada situs resminya [disini](https://www.minecraft.net/en-us/download/server).
* Daftar akun Ngrok [disini](https://ngrok.com/).

> Pastikan versi minecraft kalian sama dengan versi server minecraft agar berjalan dengan baik.

Jika sudah maka langkah pertama adalah dengan extract file Minecraft server yang kalian unduh sebelumnya dan taruh pada direktori yang kalian inginkan atau mudah ditemukan. akses folder tersebut melalui CMD jika dari Windows dan start server Minecraft, commandnya kurang lebih sebagai berikut.

    java -jar server.jar --world m-server

<a href="https://ik.imagekit.io/dsg/m-server_aAVedRiqJ.png" class="glightbox">
<img src="https://ik.imagekit.io/dsg/m-server_aAVedRiqJ.png" alt="minecraft server" />
</a>

setelah memulai server maka pada log command line kalian akan melihat port yang digunakan oleh server, simpan port tersebut yang nantinya akan digunakan pada Ngrok.

    [20:39:21] [Server thread/INFO]: Starting Minecraft server on *:25565