---
layout: post
title: Modifing File and Folder in Linux
date: 2018-10-27 +0700
description: modifikasi file dan folder di linux # Add post description (optional)
img: post-5.jpg # Add image post (optional)
tags: [Blog, Linux]
author: Averoes Blog # Add name author (optional)
---

# Mengenal jenis user di linux

   Di linux User terbagi menjadi 3, yaitu:

1.User  : Username orang yang memiliki file (owner).

2.Group : Groupuser yang memiliki hak akses yang sama terhadap file.

3.Other : Pengguna yang bukan owner dan group.

# Jenis - jenis hak akses 

   Hak akses di linux terbagi menjadi 2,yaitu :

1.Hak akses pada file.

2.Hak akses pada folder.

### 1.Hak akses pada file 

1.read (r)    : Dapat dibuka dan dibaca.

2.write (w)   : Dapat di modifikasi.

3.execute (x) : Dapat dijalankan.

### 2.Hak akses pada folder

1.read (r)   : Dapat membaca daftar file yang ada di dalam folder tsb.

2.write (w)  : Dapat mengubah atau membuat file di dalam folder tsb.

3.execute (x): Dapat mengakses file yang ada di dalam folder.

# Memodifikasi File atau Folder 

  Memodifikasi file atau folder di linux ada 2 cara:

### 1.Simbolik 

    chmod (jenis-user) + / - (ijin-hak-akses) (nama-folder/file)

contoh : 

    chmod o-r text.txt

Jenis Pengguna :

* u = user
* g = group 
* o = other 
* a = all user 

### 2.Numerik 

    chmod (angka-user)(angka-group)(angka-other) (nama-file)

contoh :

    chmod 755 text.txt

Angka :

* r = 4
* w = 2
* x = 1
* \- = 0 

Angka 755 pada contoh berasal dari 
  - r + w + x = 7 (untuk user).
  - r + x     = 5 (untuk group)
  - r + x     = 5 (untuk other)

Mungkin segitu dulu untuk materi linux yang bisa gw kasih sisanya menyusul.