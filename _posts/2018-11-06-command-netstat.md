---
layout: post
title: Fugsi dan Parameter Command Netstat
date: 2018-11-06 +0700
description: fungsi command netstat 
img: post-5.jpg # Add image post (optional)
tags: [Blog, Linux]
author: Averoes Blog # Add name author (optional)
---

# Netstat (Network Static)

  Berfungsi untuk menampilkan informasi lalu lintas transfer data dalam
  sebuah computer, command ini akan menampilkan keluar masuk data, routing table dan informasi interface jaringan.

- `netstat -a` = menampilkan semua port yang sedang terbuka 
- `netstat -at` = menampikan semua port TCP yang terbuka 
- `netstat -au` = menampilkan semua port UDP yang terbuka
- `netstat -l` = menampilkan semua socket yang terbuka 
- `netstat -lt` = menampilkan semua socket TCP yang terbuka
- `netstat -lu` = menampilkan semua socket UDP yang terbuka
- `netstat -s`  = menampilkan statistik protocol
- `netstat -st` = menampilkan staistik protocol TCP
- `netstat -su` = menampilkan statistik protocol UDP
- `netstat -pt` = menampilkan PID dan nama program
- `netstat -r` = menampilkan informasi kernel routing pada jaringan 
- `netstat -ap | grep (nama port yang sedang digunakan)` = menemukan port yang sedang di gunakan
- `netstat -i` = menampilkan informasi interface yang kita gunakan 
- `netstat -n` = menampilkan alamat dalam bentuk ip
- `netstat -o` = menampilkan timer
- `netstat -g` = menampilkan berdasarkan group membership







