---
layout: page
title: Vless WS
permalink: "/vless-ws/"
image: assets/images/file.jpg
---

```
proxies:
- name: Vless WS (SNI)
  server: SERVER.COM
  port: 443
  type: vless
  uuid: UUID
  cipher: auto
  tls: true
  skip-cert-verify: true
  servername: BUGSNI.COM
  network: ws
  ws-opts:
    path: /PATH
    headers:
      Host: BUGSNI.COM
```