---
layout: post
title: Apa itu activity pada android
date: 2019-01-29 +0700
description: teori activity pada android activity android android
img: app.png # Add image post (optional)
tags: [Blog, Android]
author: Averoes Blog # Add name author (optional)
---

## Activity itu apa sih??
  Mungkin bagi kalian yang belum pernah mendengar kata "activity" akan mencoba untuk menerka-nerka, itu makanan apa sih, rasanya enak ga ya??
  tapi bukan itu ya.

  Activity adalah sebuah tempat untuk menampilkan UI atau User Interface dari sebuah aplikasi tanpa adanya activity UI tidak akan bisa ditampilkan, lihat gambar di bawah

  ![](..assets/img/android/ui.png)

  Pada gambar tersebut ada beberapa gambar atau view-view yang ditampilkan dalam sebuah device, nah komponen untuk menampilkan view tersebut dinamakan activity.

  Oke daripada bingung kita langsung aja buat sebuah apliksi android sederhana.

  Kita akan membuat sebuah aplikasi untuk menghitung volume balok, berikut tampilannya.

  ![](..assets/img/android/mockup.png)

#### First Step

  Buka Android Studio lalu pilih File -> New -> New Project

  ![](..assets/img/android/newproject.png)

#### Second Step

  Pada bagian ini kita akan memilih tipe activity awal dari template yang telah disediakan.

 Saat ini Android Studio sudah menyediakan berbagai macam template activity dari yang paling sederhana hingga yang paling kompleks
 seperti:

Add No Activity : Tidak ada activity yang ditambahkan.

Basic Activity : Activity dengan template komponen material design seperti FloatingActionButton.

Bottom Navigation Activity : Activity dengan tampilan side bar menu di bagian bawah.

Empty Activity : Activity dalam bentuk yang paling dasar.

Fragment + ViewModel : Activity dengan menerapkan architecture component.

Fullscreen Activity : Activity fullscreen tanpa status bar.

Google AdMob Ads Activity : Activity dengan konfigurasi default iklan Admob.

Google Maps Activity : Activity dengan menyediakan konfigurasi dasar Google Maps.

Login Activity : Activity untuk halaman login.

Master / Detail Flow : Activity yang diperuntukan untuk alur aplikasi master detail pada peranti tablet.

Navigation Drawer Activity : Activity dengan tampilan side bar menu.

Scrolling Activity : Activity dengan kemampuan scroll konten didalamnya secara vertikal.

Settings Activity : Activity yang diperuntukan untuk konfigurasi aplikasi.

Tabbed Activity : Activity yang diperuntukan untuk menampilkan lebih dari satu tampilan, dapat digeser ke kanan dan ke kiri (swipe) dan dengan menggunakan komponen [ViewPager](https://developer.android.com/reference/android/support/v4/view/ViewPager).

Selain itu, Anda juga bisa memilih target device mana yang akan Anda buat seperti Phone and Tablet, Wear OS, TV, Android Auto atau Android Things.

![](..assets/img/android/template.png)

Saat ini kita pilih tipe Empty Activity, klik Next untuk melanjutkan.
