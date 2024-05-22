---
layout: page
title: Vless WS CDN
permalink: "/vless-ws-cdn/"
image: assets/images/file.jpg
---

```
proxies:
- name: Vless WS (CDN)
  server: IPCDN/BUGCDN.COM
  port: 443
  type: vless
  uuid: UUID
  cipher: auto
  tls: true
  skip-cert-verify: true
  servername: SERVER.COM
  network: ws
  ws-opts:
    path: /PATH
    headers:
      Host: SERVER.COM
```