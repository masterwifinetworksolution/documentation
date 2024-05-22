---
layout: page
title: Vmess WS
permalink: "/vmess-ws/"
image: assets/images/file.jpg
---

```
proxies:
- name: Vmess WS (SNI)
  type: vmess
  server: SERVER.COM
  port: 443
  uuid: UUID
  alterId: 0
  cipher: auto
  udp: true
  tls: true
  skip-cert-verify: true
  servername: BUGSNI.COM
  network: ws
  ws-opts:
    path: /PATH
    headers:
      Host: BUGSNI.COM
```