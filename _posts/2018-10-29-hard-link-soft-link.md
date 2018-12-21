---
layout: post
title: Penggunaan Hard Link dan Soft Link 
date: 2018-10-27 +0700
description: hard link dan soft link di linux
img: post-5.jpg # Add image post (optional)
tags: [Blog, Linux]
author: Averoes Blog # Add name author (optional)
---

# Perbedaan hard link dan soft link

  *Hard link* dan *Soft link* secara penggunaan sama,akan tetapi berbeda fungsi.Hard link bisa digunakan untuk memback up data karna isi data akan mengikuti data aslinya.Sedangkan soflink bisa digunakan untuk membuat shortcut link.

#### Hard Link bisa berdiri sendiri tanpa harus ada file aslinya.
#### Soft Link akan rusak apabila file aslinya terhapus atau namanya di rubah.

## Hard Link 

    ln (lokasi-file) (nama-link)

contoh

    ln data/file.txt file

## Soft Link

    ln -s (lokasi-file) (nama-link)

contoh

    ln -s data/file.txt file


# Menghapus link

  Menghapus link ada dua cara 

## 1.Menggunakan unlink

    unlink (nama-link)

## 2.Menggunaka rm 

    rm (nama-link)

    
Nah bagi pengguna dapat di sesuaikan mana yang dibutuhkan
Semoga Bermanfaat.
