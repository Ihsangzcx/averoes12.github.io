---
layout: post
title: Merubah Ip Dynamic ke Static
date: 2018-11-05 +0700
description: ganti ip dinamik ke statik
img: post-5.jpg # Add image post (optional)
tags: [Blog, Linux]
author: Averoes Blog # Add name author (optional)
---

# Merubah IP Dynamic jadi Static 

#### Pertama Edit file insterfaces yang berada di directory `/etc/network`

#### Lalu ubah tulisan dhcp menjadi static

#### Lalu isikan tulisan dibawah ini ke dalam nya

    adress (alamat.ip)
    netmask (255.255.255.0)
    gateway (127.0.0.1)