---
title: Vmess WS Non TLS
tags: [proxies]
keywords: account, proxies, clash
summary: "Akun clash vmess ws non tls."
sidebar: clash
permalink: vmess_ws_nontls.html
folder: proxies
comments: false
toc: false
---

```yaml
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

{% include links.html %}