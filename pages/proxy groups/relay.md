---
title: Bridge
tags: [proxy_groups]
keywords: proxy groups, relay, clash
summary: "Proxy groups relay clash."
sidebar: clash
permalink: proxy_groups_relay.html
folder: proxy groups
comments: false
toc: false
---

```yaml
proxy-groups:
- name: Select
  type: relay
  proxies: # ini bisa mengarah ke proxy group lain atau langsung di akun yang ada di config
  - trojan
  - vmess
  - vless
  - shadowsocks
  use: # ini di peruntukkan untuk jalur proxy provider
  - wan
  - wanb
```

{% include links.html %}