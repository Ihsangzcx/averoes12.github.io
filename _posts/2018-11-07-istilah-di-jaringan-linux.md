---
layout: post
title: Istilah - istilah Jaringan di Linux
date: 2018-11-07 +0700
description: state proto local adress foreign adress
img: post-5.jpg # Add image post (optional)
tags: [Blog, Linux]
author: Averoes Blog # Add name author (optional)
---

# Mengenal istilah - istilah jaringan di linux

### PROTO = Jenis Protokol

### LOCAL ADRESS = Alamat dan nomer port aktif yang ada di PC 

### FOREIGN ADRESS = Alamat yang di tuju oleh local adress

### STATE = Status dari koneksi yang terjadi 

# Macam - macam kondisi state

- LISTENING  = Siap melakukan koneksi.
- SYN_SENT   = Mengirim SYN (socket berusaha menjalin koneksi).
- SYN_RECEIVED = Menerima paket SYN (request koneksi sudah diterima dari   
                 network).
- ESTABLISHED = Koneksi terjadi dan siap mengirimkan data.
- TIME_WAIT = Sedang menunggu koneksi (socket menunggu setelah close untuk
              menagani paket yang masih di network).
- CLOSE_WAIT = Sedang menunggu menutup koneksi.
- CLOSE      = Koneksi di tutup (sisi remote sudah shutdown,menuggu socket
               close).
- FIN_WAIT1 = Socket close dan koneksi shutdown.
- FIN_WAIT2 = Socket close dan socket menunggu sisi remote shutdown.
- LAST_ACK = Sisi remote sudah shutdown socket sudah close menuggu ACK.


Mungkin hanya segitu yang saya tau jika ada yang ingin menambahkan bisa hubungi lansgsung kontak saya.

Trims...










