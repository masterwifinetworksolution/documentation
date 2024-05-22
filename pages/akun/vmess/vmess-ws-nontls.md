---
layout: page
title: Vmess WS Non TLS
permalink: "/vmess-ws-nontls/"
image: assets/images/file.jpg
---

```
proxies:
- name: Vmess WS (CDN) Non TLS
  type: vmess
  server: IPCDN/BUGCDN.COM
  port: 80
  uuid: UUID
  alterId: 0
  cipher: auto
  udp: true
  tls: false
  skip-cert-verify: false
  servername: SERVER.COM
  network: ws
  ws-opts:
    path: /PATH
    headers:
      Host: SERVER.COM
```