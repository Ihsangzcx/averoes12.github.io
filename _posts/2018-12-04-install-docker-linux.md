---
layout: post
title: Install Docker di linux
date: 2018-12-04 +0700
description: install docker linux
img: post-5.jpg # Add image post (optional)
tags: [Blog, Linux]
author: Averoes Blog # Add name author (optional)
---
# Pengenalan Docker
 Docker adalah sebuah aplikasi yang bersifat open source yang berfungsi sebagai wadah/container untuk mengepak/memasukkan sebuah software secara lengkap beserta semua hal lainnya yang dibutuhkan oleh software tersebut dapat berfungsi. Pengaturan software beserta file/hal pendukung lainnya akan menjadi sebuah Image (istilah yang diberikan oleh docker). Kemudian sebuah instan dari Image tersebut kemudian disebut Container.

# Install Docker

### First Step

Setting Repository Docker di ubuntu dengan perintah berikut

    sudo apt update
    sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    software-properties-common

### Second Step

Install GPG Key

`curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -`

### Third Step

Sekarang kita akan menginstall Docker versi CE (Community Edition),versi ini adalah versi stabil untuk ubuntu 18.04

    sudo add-apt-repository \
    "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
    $(lsb_release -cs) \
    stable"

lalu update repository anda

`sudo apt update`

lalu install docker

`sudo apt install docker ce`

Lalu kita check apakah docker sudah terisntall dengan benar atau belum

`docker --version`

# Running docker

Dengan docker kita bisa menginstall os tanpa harus dualboot

install os yang kita inginkan

`docker pull nama-os`

melihat image yang terisntalldi Docker

`docker images`

menjalankan os yang kita Install

`docker run -it nama-os bash`

untuk menghapus images

`docker rmi nama-image`


Mungkin sekian dulu dari saya

Semoga Bermafaat

Trimss..
