---
title: Shadowsocks Plugin OBFS
tags: [proxies]
keywords: account, proxies, clash
summary: "Akun clash shadowsocks plugin obfs."
sidebar: clash
permalink: shadowsocks_plugin_obfs.html
folder: proxies
comments: false
toc: false
---

```yaml
proxies:
- name: Shadowsocks Plugin Obfs
  type: ss
  server: SERVER.COM
  port: 32033
  cipher: chacha20-ietf-poly1305
  password: PASSWORD
  plugin: obfs
  plugin-opts:
    mode: tls
    host: BUGSNI.COM
```

{% include links.html %}