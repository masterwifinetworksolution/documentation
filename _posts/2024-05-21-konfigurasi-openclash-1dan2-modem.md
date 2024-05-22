---
layout: post
title:  "Konfigurasi openclash 1 dan 2 modem"
author: yusuf
categories: [ clash ]
image: assets/images/post/konfigurasi-open-clash-1dan2-modem.jpg
---

> Konfigurasi ini bisa untuk mode `script` dan juga mode `meta`. Sehingga konfigurasi ini multo fungsi.

Mari kita lihat isi dalam file yang akan saya bagikan khusus untuk anda:

### Struktur Single

```
openclash
|
|___ backup
|      |___ simaster.yaml
|
|___ config
|      |___ simaster.yaml
|
|___ core
|      |___ clash
|      |___ clash_meta
|      |___ clash_tun
|
|___ custom
|
|___ game_rules
|
|___ history
|      |___ simaster.db
|
|___ proxy_provider
|      |___ modem1.yaml
|
|___ rule_provider
|      |___ Bank.yaml
|      |___ Chat.yaml
|      |___ Game.yaml
|      |___ Iklan1.yaml
|      |___ Iklan2.yaml
|      |___ Iklam3.yaml
|      |___ Olshop.yaml
|      |___ Porn.yaml
|      |___ Sosmed.yaml
|      |___ Stream.yaml
|
|___ Country.mmdb
|
|___ GeoIP.dat
|
|___ GeoSite.dat
|
|___ accelerated-domains.china.conf
|
|___ cache.db
|
|___ china_ip6_route.ipset
|
|___ china_ip_route.ipset
|
|___ clash
|
|___ openclash
|
|___ simaster.yaml
```

Untuk mendapatkan file ini, anda bisa melalui [Disini](https://github.com/yusuftutorial/openclash/raw/master/Simaster-Backup-20Mei2024.tar.gz).

### Struktur Loadbalance

```
openclash
|
|___ backup
|      |___ simaster.yaml
|
|___ config
|      |___ simaster.yaml
|
|___ core
|      |___ clash
|      |___ clash_meta
|      |___ clash_tun
|
|___ custom
|
|___ game_rules
|
|___ history
|      |___ simaster.db
|
|___ proxy_provider
|      |___ modem1.yaml
|      |___ modem2.yaml
|
|___ rule_provider
|      |___ Bank.yaml
|      |___ Chat.yaml
|      |___ Game.yaml
|      |___ Iklan1.yaml
|      |___ Iklan2.yaml
|      |___ Iklam3.yaml
|      |___ Olshop.yaml
|      |___ Porn.yaml
|      |___ Sosmed.yaml
|      |___ Stream.yaml
|
|___ Country.mmdb
|
|___ GeoIP.dat
|
|___ GeoSite.dat
|
|___ accelerated-domains.china.conf
|
|___ cache.db
|
|___ china_ip6_route.ipset
|
|___ china_ip_route.ipset
|
|___ clash
|
|___ openclash
|
|___ simaster.yaml
```

Untuk mendapatkan file ini, anda bisa melalui [Disini](https://github.com/yusuftutorial/openclash/raw/master/Simaster-Loadbalance-20Mei2024.tar.gz).

### Cara pemasangan

1. Ekstrak File (Pilih salah satu file dari 2 yang saya sediakan).
1. copy folder `openclash` dan tempelkan ke `/etc` di dalam file manager openwrt.
1. Atur `akun` di folder `proxy_provider` untuk file `modem1.yaml` dan `modem2.yaml`.
1. Pastikan `akun` kalian sudah terhubung dengan interface modem kalian di `interface-name:`.
1. Masuk ke `openclash` dan jalankan dengan menekan `Switch Config`.