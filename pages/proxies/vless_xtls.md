---
title: Vless XTLS
tags: [proxies]
keywords: account, proxies, clash
summary: "Akun clash vless xtls."
sidebar: clash
permalink: vless_xtls.html
folder: proxies
comments: false
toc: false
---

```yaml
proxies:
- name: Vless XTLS (SNI)
  server: SERVER.COM
  port: 443
  type: vless
  uuid: UUID
  cipher: auto
  tls: true
  flow: xtls-rprx-direct
  skip-cert-verify: true
  servername: BUGSNI.COM
```

{% include links.html %}