---
title: ShadowsocksR
tags: [proxies]
keywords: account, proxies, clash
summary: "Akun clash shadowsocksr."
sidebar: clash
permalink: shadowsocksr.html
folder: proxies
comments: false
toc: false
---

```yaml
proxies:
- name: ShadowsocksR (SNI)
  server: SERVER.COM
  port: 1235
  type: ssr
  cipher: AES-256-CTR
  password: PASSWORD
  protocol: origin
  obfs: tls1.2_ticket_auth
  protocol-param: "#"
  obfs-param: BUGSNI.COM
  udp: true
```

{% include links.html %}