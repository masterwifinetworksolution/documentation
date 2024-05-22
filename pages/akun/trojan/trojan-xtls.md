---
layout: page
title: Trojan XTLS
permalink: "/trojan-xtls/"
image: assets/images/file.jpg
---

```
proxies:
- name: Trojan XTLS SNI
  server: SERVER.COM
  port: 443
  type: trojan
  password: PASSWORD
  flow: xtls-rprx-direct
  skip-cert-verify: true
  sni: BUGSNI.COM
  udp: true
```