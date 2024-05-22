---
layout: page
title: Vmess WS CDN
permalink: "/vmess-ws-cdn/"
image: assets/images/file.jpg
---

```
proxies:
- name: Vmess WS (CDN)
  type: vmess
  server: IPCDN/BUGCDN.COM
  port: 443
  uuid: UUID
  alterId: 0
  cipher: auto
  udp: true
  tls: true
  skip-cert-verify: true
  servername: SERVER.COM
  network: ws
  ws-opts:
    path: /PATH
    headers:
      Host: SERVER.COM
```