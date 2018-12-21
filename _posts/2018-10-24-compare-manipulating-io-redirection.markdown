---
layout: post
title: Compare and Manipulating File Content
date: 2018-10-24 +0700
description: manipulasi isi file di linux # Add post description (optional)
img: post-5.jpg # Add image post (optional)
tags: [Blog, Linux]
author: Averoes Blog # Add name author (optional)
---

## Manipulating file content di linux

Melihat isi file 

	cat (nama-file)
	$cat data.txt
	data1 data2 data 3
  Atau
	less (nama-file)
	$less data.txt
	data1 data2 data3
	END
 Jika ingin keluar tekan q

Mengurutkan File

	sort (nama-file)
	$sort data.txt
	data1
	data2
	data3

	sort -r = reverse atau kebalikan mengurutkan dari bawah ke atas
	sort -n = mengurutkan dari 0
	sort -M = mengurutkan bulan
	sort -v = mengurutkan versi
  
  Bisa dilihat di `man sort`

Melihat 10 Baris Pertama 

	head (nama-file)

Melihat 10 baris terakhir

	tail (nama-file)

## Using Input Output Redirection

Membuat file baru

	sort (nama-file) > (nama-file2)
isi file yang ada di `nama-file` di sort lalu di masukkan ke dalam file `nama-file2`

	
	$sort data.txt >  list.txt 
	$cat list.txt
	data1
	data2
	data3

Menambahkan file 

	sort data2.txt >> list.txt
Isi file yang ada di `data2.txt` di tambahkan ke dalam file `list.txt`.

	$sort data2.txt >> list.txt
	$cat list.txt
	data1
	data2
	data3
	file
	file2
	file3


