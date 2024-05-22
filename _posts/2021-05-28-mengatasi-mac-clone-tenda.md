---
layout: post
title:  "Mengatasi mac clone router tenda"
author: yusuf
categories: [ router ]
image: assets/images/post/atasi-mac-clone-tenda.jpg
---
Untuk bisa menghilangkan pemberitahuan `Clone Mac Address` pada router `Tenda`, maka anda wajib melakukan hal di bawah ini:

1. Masuk ke router `Tenda`.
1. Lakukan login.
1. Pergi pengaturan `Administration`.
1. Ubah Mac ke `Manual`.
1. Salin `Mac Address` yang ada di router utama ke tempelkan ke Mac Address Tenda.
1. Tekan `Save`.

Jika masih muncul kembali `Clone Mac Address`, maka lakukan hal di bawah ini lagi.

- Tetap berada di router `Tenda`.
- Pergi ke pengaturan `Internet Setting`
- Ubah `DHCP` menjadi `Static IP`

```txt
Address: xxx.xxx.xxx.xxx # isikan ip untuk tenda
Subnet Mask: 255.255.255.0 # sesuaikan dengan subnet modem utama
Gateway: xxx.xxx.xxx.x # sesuaikan dengan alamat ip router utama dan sama dengan address juga
dns primary: xxx.xxx.xxx.x # samakan saja dengan alamat gateway
```

- Jika sudah semua beres, tinggal lakukan `save`.