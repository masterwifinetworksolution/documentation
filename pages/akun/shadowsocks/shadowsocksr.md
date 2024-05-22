---
layout: page
title: ShadowsocksR
permalink: "/shadowsocksr/"
image: assets/images/file.jpg
---

```
proxies:
- name: ShadowsocksR (SNI)
  server: SERVER.COM
  port: 1235
  type: ssr
  cipher: AES-256-CTR
  password: PASSWORD
  protocol: origin
  obfs: tls1.2_ticket_auth
  protocol-param: "#"
  obfs-param: BUGSNI.COM
  udp: true
```