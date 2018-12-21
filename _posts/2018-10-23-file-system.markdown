---
layout: post
title:  Penjelesasan File System di Linux
date:   2018-10-23 +0700
description: file system di linux# Add post description (optional)
img: post-5.jpg # Add image post (optional)
tags: [Blog, Linux]
author: Averoes Blog # Add name author (optional)
---

# File system 

  File system merupakan database yang digunakan untuk mengelola data yang ada pada laptop atau pc kita,file system juga meruapakan sebuah interface untuk menghubungkan OS dengan File, agar User  dapat melihat file tersebut.

# Jenis-jenis file system 

###  1.Ext

Ext atau Extended File System merupakan jenis file system yang di perkenalakan pada tahun 1992,Ext mempunyai beberapa versi :

 1.Ext2 (Second Extended)

  Ext2 merupakan file system yang paling banyak digunakan di OS linux,file system ini menyimpan data yang banyak digunakan oleh system operasi.

 2.Ext3 (Third Extended)

  Ext3 merupakan file system yang ditingkatkan dari Ext2,diantaranya :

   => Journaling

   Dengan menggunakan journaling estimasi waktu saat recovery data ketika shutdown mendadak tidak akan selama Ext2,akan tetapi akan memperlambat system Input/Output karna mebutuhkan banyak memori.

   => Integritas Data

   Menjamin adanya integritas data setelah terjadi kerusakan atau unclean shtudown.

   => Kecepatan 

   Ext3 mempunyai throughput yang lebih besar dari Ext2,karna Ext3 memaksimalkan pergerakan head hard disk.

   => Mudah migrasi

   Kita bisa berpindah dari Ext3 ke Ext2 tanpa harus format ulang.

###  Ext4 (Fourth Extended File System)
   
Ext4 merupakan peningkatan dari file system ext2 dan ext3 yang dirilis secara lengkap dan stabil.

### JFS (Journaling File System)

JFS merupakan file sistem pertama yang menawarkan journaling pertama,JFS menjadi file system yang paling sedikit menggunakan sumber daya CPU dibandingkan sistem file GNU/Linux lainnya.JFS sangat cepat diformat ,mounting,dan fsck,serta memiliki kinerja sangat baik.

### XFS
     
XFS mempunyai throughput yang sangat cepat pada file besar, dan sangat cepat di format dan mounting akan tetapi throughput nya lambat pada file kecil.

### BTRFS (B-Tree File System)
 
BTRFS merupakan file system yang berada di bawah lisensi General Public Lisence.
BTRFS membuat linux dapat lebih mengatur storage yang ada dan juga dapatmelakukan administrasi dan pengelolaan tempat penyimpanan dengan interface yang lebih bersih.

### ZFS (Zettabytes File System)

ZFS merupakan file system terbaru yang dikembangkan oleh Sun,yang dirancang untuk menggunakan metode penyimapanan yang dikumpulkan(pooling).Dan juga telah dirancang unutk integritas data maksimum,mendukung snapshot data ,multiple penyalinan,dan checksum data.



==> Sumber https://www.lk21.new/2016/07/penjelasan-lengkap-file-sistem-linux.html