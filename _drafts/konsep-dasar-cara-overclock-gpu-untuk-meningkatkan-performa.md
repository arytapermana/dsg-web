---
layout: post
author: sal
date: 2021-04-17 07:36:31 +0800
title: Konsep Dasar Cara Overclock GPU Untuk Meningkatkan Performa
categories:
- Info
tags:
- GPU
- Overclock
image: https://ik.imagekit.io/dsg/overclock_c0S9sbRb0hk.jpg

---
Overclocking adalah hal yang cukup banyak diperdebatkan dalam aspek penggunaan sehari hari, diingatkan lagi sehari-hari, bukan tingkat kompetisi, hal ini dikarenakan sebagian menganggap overclocking dapat merusak komponen yang ada pada perangkat hardware karena meningkatkan clock atau frekuensi yang ada diluar pengaturan pabrikannya sedangkan pihak lain mengaggap overclocking tetap aman digunakan sehari-hari jika pengaturan frekuensi ataupun suhu yang ada tetap terjaga. kali ini kami tidak akan membahas hal tersebut tetapi kami akan membahas konsep dasar overclocking khususnya GPU atau graphics card untuk pemakaian sehari-sehari, perlu diingat _Do at your own risk._

Sebelum memulai tahapan yang ada, berikut beberapa hal yang perlu dipersiapkan untuk melakukan overclocking.

* GPU/Graphics Card (OC/Overclock Version)

  Pastikan graphics card yang kalian miliki adalah versi yang dapat dilakukan overclock, kami tidak membahas bagaimana mengetahuinya, biasanya vendor telah memberitahukannya di awal.
* [MSI Afterburner](https://www.msi.com/Landing/afterburner) (Software OC)

  Sebenarnya tidak hanya MSI Afterburner software yang dapat digunakan untuk melakukan overclock gpu kalian, tetapi software satu ini yang cukup banyak digunakan, _user friendly_ dan fitur yang ada cukup lengkap.
* [Heaven Benchmark](https://benchmark.unigine.com/heaven) (Software Benchmark)

  Untuk melakukan benchmark kami menggunakan Heaven Benchmark dikarenakan ukuran yang cukup ringan dan testing skenario yang lebih mendekati gaming, selain Heaven Benchmark kalian dapat menggunakan [3DMark](https://www.3dmark.com/). Untuk Benchmark seperti [MSI Kombustor](https://geeks3d.com/furmark/kombustor/) atau [FurMark](https://geeks3d.com/furmark/) lebih mendekati skenario untuk melakukan testing GPU hingga mendekati _limit_ terakhir dimana game tidak berada di skenario ini.

## Tahapan Overcloking GPU

Jika hal-hal yang telah disebutkan sebelumnya sudah siap maka kita dapat lanjut ke tahapan overclocking, mohon membaca dengan perlahan agar tidak ada informasi yang terlewat karena semua tahapan harus berjalan dengan baik untuk mendapatkan pefroma dan stabilitas terbaik juga, perlu diingat performa yang dihasilkan tidak selalu sama, walaupun graphics card yang ada sama persis, karena setiap hardware memiliki proses manufacture yang tidak selalu sama, hal ini hampir sama seperti _silicon lottery_ pada CPU.

### MSI Afterburner

![](https://ik.imagekit.io/dsg/1_28KsAyahNuP.png)

Sebelum melakukan _tweaking_ dan _tunning_ pada GPU kalian, perlu diketahui dulu fungsi-fungsi dari _tools_ yang disediakan oleh MSI Afterburner walaupun terlihat mengintimidasi, pengaturan tersebut sebenarnya cukup mudah diingat. Mungkin tampilan yang ada cukup berbeda dari yang kalian miliki tetapi _tools_ yang ada tetap sama hanya berbeda posisi. Berikut beberapa penjelasan singkat tools tersebut.

* **Core Voltage**, Adalah pengaturan voltase yang diberikan kepada graphics card itu sendiri.
* **Core Clock**, Jumlah yang perlu ditambah atau dikurangi dari base Frekuensi pada Core GPU.
* **Memory Clock**, Jumlah yang perlu ditambah atau dikurangi dari base Frekuensi pada Memory GPU.
* **Power Limit**, Jumlah sumber daya yang dialokasikan kepada graphics card.
* **Temp Limit**, Target maksimum suhu dari graphics card itu sendiri.
* **Fan Speed**, Kecepatan kipas pada graphics card.

### Tweaking/Tunning Core Clock

Penyetelan yang pertama adalah mencari _core clock_ yang stabil dari _graphics card_ yang kalian miliki, hal ini dapat dilakukan dengan cara meningkatkan frekuensi sedikit demi sedikit seperti menambahkan +10Mhz hingga +50Mhz sambil menjalan Heaven Benchmark, dan ketika terasa benchmark yang ada mengalami stutter, lagging, artifact, ataupun hingga drop pada framerate yang ada maka turunkan frekuensi tersebut hingga mendapatkan performa yang stabil.