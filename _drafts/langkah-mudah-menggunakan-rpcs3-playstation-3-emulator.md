---
layout: post
author: sal
date: 2021-05-06 16:11:39 +0800
title: Langkah Mudah Menggunakan RPCS3 - PlayStation 3 Emulator
categories:
- Info
tags:
- 'RPCS3 '
- PlayStation
- Emulator
image: https://ik.imagekit.io/dsg/thumb_1__-L2pAC1pv.jpg

---
PlayStation 3, begitu banyak nostalgia game yang ada, bagi kalian yang telah memainkan game pada konsol satu ini. Jadi kali ini kami akan memberikan tahapan untuk setup atau menyiapkan RPCS3 yaitu emulator PlayStation 3 yang cukup cepat perkembangannya waktu demi waktu dari segi optimalisasi.

> Legalitas emulator konsol game masih dipertanyakan hingga sekarang, walaupun firmware resmi dan game yang ada dapat di extract langsung dari cd gamenya tetap masih ada celah yang dipertanyakan.

Langsung saja, sebelum itu kalian perlu melakukan download beberapa kebutuhannya terlebih dahulu, beberapa hal tersebut adalah sebagai berikut.

* [RPCS3](https://rpcs3.net/download), tentu emulatornya itu sendiri, kalian dapat mengunduhnya pada situs RPCS3.
* [Firmware](https://www.playstation.com/en-us/support/hardware/ps3/system-software/), dalam menjalankan sistemnya RPCS3 memerlukan firmware dari PlayStation 3 itu sendiri, kalian dapat mengunduhnya pada situs resmi PlayStation.

Jika semua hal yang dibutuhkan sudah siap maka kita dapat lanjut ke tahapan berikutnya.

## RPCS3

Setelah kalian mengunduh emulatornya kalian dapat membuka rpcs3.exe langsung karena tidak memerlukan instalasi pada sistem operasi, setelah membuka RPCS3, lakukan instalasi firmware pada menu terlebih dahulu.

<a href="https://ik.imagekit.io/dsg/1_FMRLU4K6p.png" class="glightbox">
<img src="https://ik.imagekit.io/dsg/1_FMRLU4K6p.png" alt="image" />
</a>

Pilih file firmware yang telah diunduh sebelumnya kemudian tunggu proses instalasinya

## Play

Setelah langkah sebelumnya selesai seharusnya kalian telah dapat memainkan game pada RPCS3. Untuk memainkan game yang ada kalian hanya perlu memilih menu File kemudia klik Boot Game dan arahakan menuju direktori game yang ada dan Select Folder.

> Dari mana mendapatkan game?, kalian dapat melakukan extract cd game playstation yang ada dan tutorialnya telah disediakan pada dokumentasi RPCS3 [berikut](https://rpcs3.net/quickstart). <span class="spoiler">Atau kalian bisa download pada situs yang telah menyediakan ROM game PlayStation 3 (kami tidak sarankan, mungkin hal ini ilegal).</span>

<a href="https://ik.imagekit.io/dsg/2_9s9DE4-Ro.png" class="glightbox">
<img src="https://ik.imagekit.io/dsg/2_9s9DE4-Ro.png" alt="image" />
</a>

Jika sudah maka semua tahapan telah selesai dan selamat bermain ataupun bernostalgia, ups.. ada satu hal lagi tetapi opsional yang akan dibahas selanjutnya dibawah.

## Tweaking

Sistem yang dibutuhkan untuk menjalankan emulator sebenarnya cukup berat, dilansir dari situs RPCS3 jumlah processor cores minimal adalah lebih dari 4 cores, atau untuk processor pada kelas Intel Core i5 atau AMD Ryzen 3 dan kebawah memiliki sedikit masalah menjalankan emulator ini, tetapi kami memiliki beberapa tweaking yang dilansir dari post [Reddit](https://www.reddit.com/r/rpcs3/comments/kdy4w7/suggestions_for_optimizing_rpcs3_for_performance/) oleh [u/arrowflask](https://www.reddit.com/user/arrowflask/) agar dapat meningkatkan stabilitas dan framerate pada emulator, sebelum itu masuk terlebih dahulu pada menu config.

<a href="https://ik.imagekit.io/dsg/3_1X3TJAsQU.png" class="glightbox">
<img src="https://ik.imagekit.io/dsg/3_1X3TJAsQU.png" alt="image" />
</a>

setelah muncul jendela baru maka aturlah beberapa settings yang akan dijelaskan berikut.

### CPU tab:

* Preferred SPU Threads (Auto): **3 atau 2**
* Lower SPU Thread Priority (Disabled): **Enabled**
* Enable SPU Loop Detection (Enabled): **Disabled**

### GPU tab:

* Shader Mode (Async multi threaded): **Async w/ Shader Interpreter**
* Number of Shader Compiler Threads: **2**

### Audio tab:

* Audio Buffer Duration (100 ms): **150 ms**

### Emulator tab:

* Max LLVM Compile Threads (4): **3**

### Advanced tab:

* Relaxed ZCULL Sync (Disabled): **Enabled** (aman untuk kebanyakan game, akan menyebabkan beberapa game tidak dapat boot atau crash pada title screen)
* Maximum Number of SPURS Threads (Unlimited == 6): **4 or 3** (jika terjadi masalah tingkatkan menjadi +1 hingga stabil)