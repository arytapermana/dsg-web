---
layout: post
author: sal
date: 2021-04-17T07:36:31.000+08:00
title: Konsep Dasar Cara Overclock GPU Untuk Meningkatkan Performa
categories:
- Info
tags:
- GPU
- Overclock
image: https://ik.imagekit.io/dsg/overclock_c0S9sbRb0hk.jpg

---
Overclocking adalah hal yang cukup banyak diperdebatkan dalam aspek penggunaan sehari hari, diingatkan lagi sehari-hari, bukan tingkat kompetisi, hal ini dikarenakan sebagian menganggap overclocking dapat merusak komponen yang ada pada perangkat hardware karena meningkatkan clock atau frekuensi yang ada diluar pengaturan pabrikannya, sedangkan pihak lain mengaggap overclocking tetap aman digunakan sehari-hari jika pengaturan frekuensi ataupun suhu yang ada tetap terjaga. kali ini kami tidak akan membahas hal tersebut tetapi kami akan membahas konsep dasar overclocking khususnya GPU atau graphics card untuk pemakaian sehari-sehari, perlu diingat Do at your own risk!.

Sebelum memulai tahapan yang ada, berikut beberapa hal yang perlu dipersiapkan untuk melakukan overclocking.

* **GPU/Graphics Card (OC/Overclock Version)**, Pastikan graphics card yang kalian miliki adalah versi yang dapat dilakukan overclock, kami tidak membahas bagaimana mengetahuinya, biasanya vendor telah memberitahukannya di awal.
* [**MSI Afterburner**](https://www.msi.com/Landing/afterburner) (Software OC), Sebenarnya tidak hanya MSI Afterburner software yang dapat digunakan untuk melakukan overclock GPU kalian, tetapi software satu ini yang cukup banyak digunakan, user friendly dan fitur yang ada cukup lengkap.
* [**Heaven Benchmark**](https://benchmark.unigine.com/heaven) (Software Benchmark), Untuk melakukan benchmark kami menggunakan Heaven Benchmark dikarenakan ukuran yang cukup ringan dan testing skenario yang lebih mendekati gaming, selain Heaven Benchmark kalian dapat menggunakan [3DMark](https://www.3dmark.com/). Untuk Benchmark seperti [MSI Kombustor](https://geeks3d.com/furmark/kombustor/) atau [FurMark](https://geeks3d.com/furmark/) lebih mendekati skenario untuk melakukan testing GPU hingga mendekati limit terakhir dimana game biasanya tidak berada di skenario ini.

## Tahapan Overcloking GPU

Jika hal-hal yang telah disebutkan sebelumnya sudah siap, maka kita dapat lanjut ke tahapan overclocking, mohon membaca dengan perlahan agar tidak ada informasi yang terlewat karena semua tahapan harus berjalan dengan baik untuk mendapatkan perfoma dan stabilitas terbaik juga, perlu diingat performa yang dihasilkan tidak selalu sama, walaupun graphics card yang ada sama persis, karena setiap hardware memiliki proses manufacture yang tidak selalu sama, hal ini hampir sama seperti silicon lottery pada CPU.

### MSI Afterburner

Sebelum melakukan tweaking dan tunning pada GPU kalian, perlu diketahui dulu fungsi-fungsi dari tools yang disediakan oleh MSI Afterburner walaupun terlihat mengintimidasi, pengaturan tersebut sebenarnya cukup mudah diingat. Mungkin tampilan yang ada cukup berbeda dari yang kalian miliki tetapi tools yang ada tetap sama, hanya berbeda posisi. Berikut beberapa penjelasan singkat tools tersebut.

![](https://ik.imagekit.io/dsg/1_28KsAyahNuP.png)

* **Core Voltage**, Adalah pengaturan voltase yang diberikan kepada graphics card itu sendiri.
* **Core Clock**, Jumlah yang perlu ditambah atau dikurangi dari base Frekuensi pada Core GPU.
* **Memory Clock**, Jumlah yang perlu ditambah atau dikurangi dari base Frekuensi pada Memory GPU.
* **Power Limit**, Jumlah sumber daya yang dialokasikan kepada graphics card.
* **Temp Limit**, Target maksimum suhu dari graphics card itu sendiri.
* **Fan Speed**, Kecepatan kipas pada graphics card.

Tidak semua tools yang ada dapat digunakan terkadang, tergantung manufacture dari graphics card itu sendiri, seperti pada graphics card yang kami gunakan, core voltage yang ada tidak dapat diubah maupun di utak-atik walaupun pada pengaturan MSI Afterburner telah ter-unlock.

### Memulai

Sebelum masuk ke Tunning pertama, pastikan Power Limit dan Temp Limit berada pada maksimum, jangan terkejut dahulu, manufaktur telah membatasi jumlah maksimum limit power dan juga suhu yang ada untuk dapat di tunning pada versi gpu overclock, dan ini juga memiliki variasi berbeda beda, pada contoh kami, maksimum power limit adalah 100% tetapi ada juga yang dapat meningkatkannya hingga 120% pada jenis graphics card berbeda, jadi kalian masih berada pada batas relatif aman.

![](https://ik.imagekit.io/dsg/2_zEx_oYQ1_.jpg)

Jangan lupa pastikan melepas sinkronisasi link temperature dengan fan speed dengan click icon rantai hingga berstatus OFF agar ketika pengaturan disimpan tidak berubah ke default pada temp limit, selain itu agar memastikan peforma yang berjalan berada pada maksimum tidak terhambat limitasi suhu. Biarkan juga fan berjalan pada mode auto dengan icon mirip hurup "A" berada pada status ON atau terlihat bold.

![](https://ik.imagekit.io/dsg/fps_IkPIStL8MiP.jpg)

Pada saat proses tunning core clock dan memory clock pastikan kalian memantau framerate pada software benchmark, pastikan framerate tidak malah menurun dan juga selain itu pantau suhu GPU tidak melebihi 90°C walau penggunaan jangka pendek tidak ada masalah, tapi penggunaan jangka panjang akan mempercepat umur graphics card tersebut, Sekitar 70°C dan 80°C masih relatif aman, dibawah itu lebih baik lagi. untuk target tertinggi overclocking GPU biasanya frame rate yang dapat dicapai adalah 10% dari rata-rata frame rate sebelumnya, contohnya jika frame rate di awal adalah 100fps dan mendapatkan 110fps setelah overclocking maka overclocking kalian sudah dapat dianggap mencapai target.

### Tweaking/Tunning Core Clock

Tunning yang pertama adalah mencari core clock yang stabil dari graphics card yang kalian miliki, hal ini dapat dilakukan dengan cara meningkatkan frekuensi core clock sedikit demi sedikit seperti menambahkan +10Mhz hingga +50Mhz sambil menjalankan Heaven Benchmark, dan ketika terasa benchmark yang ada mengalami [stutter](https://www.youtube.com/watch?v=wmtZ07qHFS4&list=UUoAASU98g2jffZ_eHIdinug "GPU Stutter, by Alexander Stopher"), [lagging](https://www.youtube.com/watch?v=j3WvNxi-9fQ "Lagging, by The Frugal Streamer"), [artifacts](https://www.youtube.com/watch?v=q9n9i2ujwtg&t=16s "Artifacts, by Lynyrd"), ataupun hingga [drop framerate](https://www.youtube.com/watch?v=dRt3mJiETh4 "FPS Drop, by Snips86x"), maka turunkan frekuensi tersebut hingga mendapatkan performa yang stabil.

![](https://ik.imagekit.io/dsg/ezgif.com-gif-maker_NT2LfCZJ_.gif)

Pada contoh yang ada, kami telah mendapatkan core clock yang stabil berada pada +140MHz, jangan terlalu memaksa untuk meningkatkan core clock walau suhu GPU terlihat masih berada batas aman karena GPU memiliki batasannya tersendiri dan jika terlalu jauh maka Software Benchmark atau PC yang ada akan mengalami crash hingga freeze, kalian dapat merestartnya dengan normal atau dengan paksa jika tidak dapat digunakan sama sekali. Setelah hidup kembali maka semua kembali ke default lagi.

### Tweaking/Tunning Memory Clock

Langkah selanjutnya adalah mencari memory clock yang stabil, dengan cara menambahkannya sedikit demi sedikit, kalian dapat memulai dengan menambahkan +50Mhz hingga +100Mhz hingga menemukan ketidak stabilan dan kemudian turunkan sedikit demi sedikit hingga sudah terasa cukup stabil, pada contoh kali ini gpu yang kami gunakan berada pada +850Mhz dimana batas stabil dan perfoma yang didapat cukup signifkan.

![](https://ik.imagekit.io/dsg/memory-clock_9Hc1t4NbCLt.gif)

Masih sama seperti sebelumnya tetap pastikan suhu yang ada berada batas aman, peforma yang ada juga stabil. Setidaknya kalian akan melihat ada penambahan frame rate pada benchmark sebelumnya.

### Done!

Jika sudah selesai maka simpan pengaturan yang ada dengan menekan tombol save yang berbentuk icon memory card, dan pilih simpan pada profile 1 ataupun profile lainnya, serta pastikan tombol startup yang berada pada pojok kanan atas aktif untuk memastikan profile overclock berjalan saat start up.

![](https://ik.imagekit.io/dsg/save-compress_CxCPTfrBi.gif)

Maka sekarang cobalah gunakan PC kalian untuk pemakaian normal ataupun memainkan game favorit yang ada, kalian juga dapat melakukan test benchmark dari versi stock yang ada dan setelah overclock, kemudian lihat hasil perbedaan score yang didapat. Jika dirasa ada kejanggalan, seperti yang disebutkan sebelumnya, maka cobalah turunkan core clock atau memory clock, karena hal tersebut berarti sistem tidak stabil, hal ini terjadi diakibatkan setiap software yang ada memiliki penggunaan sumber daya dari GPU berbeda-beda sehingga perlu penyesuaian lagi.

Mungkin itu saja yang dapat kami sampaikan mengenai dasar-dasar overcloking GPU, jika masih ada hal yang ingin ditanyakan atau bingung, jangan sunkan untuk bertanya pada kolom komentar dibawah, Terimakasih!