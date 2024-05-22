---
layout: page
title: Trojan GFW
permalink: "/trojan-gfw/"
image: assets/images/file.jpg
---

```
proxies:
- name: Trojan GFW (SNI)
  type: trojan
  server: SERVER.COM
  port: 443
  password: PASSWORD
  udp: true
  sni: BUGSNI.COM
  skip-cert-verify: true
```