---
layout: page
title: Vless WS Non TLS
permalink: "/vless-ws-nontls/"
image: assets/images/file.jpg
---

```
proxies:
- name: Vless WS (CDN) Non TLS
  server: IPCDN/BUGCDN.COM
  port: 80
  type: vless
  uuid: 81f1f510-3ca7-4734-8956-0f4fce670af5
  cipher: auto
  tls: false
  skip-cert-verify: false
  servername: SERVER.COM
  network: ws
  ws-opts:
    path: /PATH
    headers:
      Host: SERVER.COM
  udp: true
```