---
layout: page
title: Shadowsocks OBFS
permalink: "/shadowsocks-obfs/"
image: assets/images/file.jpg
---

```
proxies:
- name: Shadowsocks Plugin Obfs
  type: ss
  server: SERVER.COM
  port: 32033
  cipher: chacha20-ietf-poly1305
  password: PASSWORD
  plugin: obfs
  plugin-opts:
    mode: tls
    host: BUGSNI.COM
```