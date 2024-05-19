---
title: Vmess WS TLS
tags: [proxies]
keywords: account, proxies, clash
summary: "Akun clash vmess ws tls."
sidebar: clash
permalink: vmess_ws_tls.html
folder: proxies
comments: false
toc: false
---

## SNI

```yaml
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

## CDN

```yaml
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

{% include links.html %}