---
layout: post
title: Transfer File dengan Terminal di Linux 
date: 2018-10-27 +0700
description: hard link dan soft link di linux
img: post-5.jpg # Add image post (optional)
tags: [Blog, Linux]
author: Averoes Blog # Add name author (optional)
---

# Transfer file atau folder lewat terminal

  Masih jaman kirim file atau folder dengan flashdisk atau HDD eksternal.
  Di linux sudah di sediakan command untuk mengirim file dari satu PC ke PC lain tanpa menggunakan flashdisk media lainnya,cukup buka terminal daan jalankan command nya file atau folder anda akan terkirim.

# Langkah - langkah 

 Pertama kita tentukan akan mengirim file yang akan kita kirim lalu ubah ownership dari file atau folder tersebut.

 Berikut command untuk merubah ownership file atau folder

    chown (nama-user) (nama-file/folder) 
contoh 

    chown -R averoes:averoes folder

Lalu setelah kita rubah ownership nya kita ketikkan command di bawah ini untuk mengirim file tersebut

    scp (nama-file/folder) (nama-user-tujuan)@(ip-tujuan):(letak-file-yang-akan-kita-letakkan)

contoh

    scp -r folder admin@123456789:/home/dokumen/data 

jika kita ingin menyamakan isi folder yang ada pada laptop/PC kita dengan laptop/PC tujuan atau mem back up foler yang kita punya ke laptop tujuan
kita bisa menggunakan command di bawah ini

    rync (nama-file/folder) (nama-user-tujuan)@(ip-tujuan):(letak-file-yang-akan-kita-letakkan)

contoh 

    rsync folder admin@123456789:/home/dokumen/data

maka folder yang ada di laptop/pc tujuan akan sama dengan yang ada pada pc /laptop kita termasuk permission nya juga.