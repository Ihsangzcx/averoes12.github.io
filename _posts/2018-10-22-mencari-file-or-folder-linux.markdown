---
layout: post
title: Mencari File Atau Folder Di Linux
date: 2018-10-22 +0700
description: cara mencari file di linux # Add post description (optional)
img: post-5.jpg # Add image post (optional)
tags: [Blog, Tutorial]
author: Averoes Blog # Add name author (optional)
---

# Mencari File Atau Folder Dengan Command find

   Sebenernya command untuk mencari file atau folder di linux  banyak,tapi kali ini yang admin akan share adalah bagaimana mencari file atau folder dengan command find.

### 1.Mencari file di folder sekarang

   Jika kita ingin mencari file yang ada didalam folder yang sedang kita tempati. 

	find -name (nama-file)

### 2.Mencari file di folder lain

   Jika kita ingin mencari file yang ada di folder tertentu.

	find ~/Dokumen/Learn <==contoh -name (nama-file)

### 3.Mencari folder 
   Jika kita ingin mencari folder 

	find -type d -name (nama-folder)

### 4.Mencari file dengan size

	find size +(size)(satuan size*)
  
  *satuan size = mb(milibyte) b(byte) Kb(Kilo byte) Mb(Mega byte) Gb(Giga byte) 

### 5.Mencari file atau folder dengan wildcart

  Jika kita lupa nama file atau folder kita bisa mencari dengan menggunakan wildcart

	find -type f -name "*.txt" <== contoh
	find -type d -name "*doc"  <== contoh

### 6.Mencari insensitive file atau folder
   
   Jika kita ingin mencari nama file atau folder tanpa memperhatikan besar kecil huruf.

	find -type f -iname (nama-file)
	find -type d -iname (nama-folder)

  Mungkin Segini dulu yang bisa admin share, karna biasanya cuma yang ini yang sering digunakan.
  Sebenarnya masih banyak lagi command-command yang lain tapi untuk kali ini segini dulu.