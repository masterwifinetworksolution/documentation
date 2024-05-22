---
layout: page
title: Socks5
permalink: "/socks5/"
image: assets/images/file.jpg
---

```
proxies:
- name: Socks5 (SNI)
  type: socks5
  server: SERVER.COM
  port: 443
  username: USERNAME
  password: PASSWORD
  tls: true
  skip-cert-verify: true
  udp: true
  sni: BUGSNI.COM
```