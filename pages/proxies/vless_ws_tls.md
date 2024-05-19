---
title: Vless WS TLS
tags: [proxies]
keywords: account, proxies, clash
summary: "Akun clash vless ws tls."
sidebar: clash
permalink: vless_ws_tls.html
folder: proxies
comments: false
toc: false
---

## SNI

```yaml
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

## CDN

```yaml
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

{% include links.html %}