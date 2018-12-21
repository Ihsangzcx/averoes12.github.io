---
layout: post
title:  Install Steam On Kali Linux
date:   2018-10-09 +0700
description: Cara Intall Steam # Add post description (optional)
img: post-4.png # Add image post (optional)
tags: [Blog, Tutorial]
author: Averoes Blog# Add name author (optional)
---

# Install Steam Di Kali Linux



Mungkin kalian berpikir kalo Kali Linux itu distro linux untuk kebutuhan pentest dan riset computer security, tapi apa gk bosen sesekali perlu hiburan nge-game misalnya? Nah, yang butuh tutorial untuk bagaimana cara menginstall Steam di Kali Linux 2.0, silakan ikuti.

Steam adalah aplikasi store dan launcher sejumlah game populer, yang bisa berjalan di Windows, Mac maupun Linux. Sebagai layaknya sebuah toko, disana sampeyan bisa beli dan mainkan game yang dibeli sepuasnya.

Nah, ini tutorial untuk menginstall Steam di Kali Linux 2.0

1.Download Steam 

Download Installer Steam
Silakan download installer Steam berupa file .deb dari situs Steam di:

https://steamcdn-a.akamaihd.net/client/installer/steam.deb

![Steam]({{site.baseurl}}/assets/img/steam.png)

2.Kemudian buka console/terminal dan ketik perintah:

1.sudo dpkg -i steam.deb

2.sudo apt install -f
 
Sebenarnya pada langkah ini seharusnya proses instalasi sudah selesai. Namun karena kita login ke Kali Linux dengan user root, maka harus ada sedikit modifikasi biar Steam jalan lancar.

3.Silakan edit file /usr/bin/steam dan temukan sintaks:

	#Don’t allow running as root
 	
	if [ "$(id -u)" == "0" ]; then
	show_message –error $”Cannot run as root user”
	exit 1<br>
	fi


lalu ganti dengan:


	#Don’t allow running as root
	if [ "$(id -u)" == "1" ]; then
	show_message –error $”Cannot run as root user”
	exit 1
	fi


4.Langkah keempat ini, khusus bagi yang menggunakan Kali Linux 64 bit, silakan lakukan langkah ini:


	dpkg --add-architecture i386
 
	sudo apt update
 
	sudo apt install libc6:i386 libqt4-dbus:i386 libqt4-network:i386
	libqt4-xml:i386 libqtcore4:i386 libqtgui4:i386 libqtwebkit4:i386
	libstdc++6:i386 libx11-6:i386 libxext6:i386 libxss1:i386 libxv1:i386
	libssl1.0.0:i386 libpulse0:i386 libasound2-plugins:i386


Selamat Mencoba...