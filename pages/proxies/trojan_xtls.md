---
title: Trojan XTLS
tags: [proxies]
keywords: account, proxies, clash
summary: "Akun clash trojan xtls."
sidebar: clash
permalink: trojan_xtls.html
folder: proxies
comments: false
toc: false
---

```yaml
proxies:
- name: Trojan XTLS (SNI)
  server: SERVER.COM
  port: 443
  type: trojan
  password: PASSWORD
  flow: xtls-rprx-direct
  skip-cert-verify: true
  sni: BUGSNI.COM
  udp: true
```

{% include links.html %}