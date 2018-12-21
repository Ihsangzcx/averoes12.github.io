---
layout: post
title: Install and Create virtual machine di QEMU dengan metode CLI
date: 2018-12-11 +0700
description: install qemu linux virtual machine
img: post-5.jpg # Add image post (optional)
tags: [Blog, Linux]
author: Averoes Blog # Add name author (optional)
---

# Qemu 

Qemu adalah virtual machine yang berbasis kvm sama seperti virtual box,namun qemu lebih ringan dari virtual box.

# Install qemu 

Pertama Update dulu

`sudo apt-get update`

lalu install qemu nya

`sudo apt install -y qemu-kvm qemu virt-manager virt-viewer libvirt-bin`

# Creating virtual machine

`sudo virt-install --name=UBUNTU --memory=1024 --vcpus=1 --os-type=linux --cdrom=ubuntu.iso --disk path=ubuntu.dsk,size=4`

setelah itu akan keluar pop up berupa GUI dari qemu 


--name = Nama Mesin virtual

--memory= Ram mesin virtual

--vcpus= Jumlah cpu virtual

--os-type = Tipe OS

--cdrom = Lokasi file iso

--disk path = Lokasi untuk menempatkan mesin virtual
size = Jumlah hard disk virtual

Untuk melihat OS yang sudah di install kita bisa menulis

`sudo virt-manager`

untuk membuka GUI qemu















