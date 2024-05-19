---
title: Loadbalance
tags: [proxy_groups]
keywords: proxy groups, loadbalance, clash
summary: "Proxy groups loadbalance clash."
sidebar: clash
permalink: proxy_groups_loadbalance.html
folder: proxy groups
comments: false
toc: false
---

```yaml
proxy-groups:
- name: LOADBALANCING
  type: load-balance
  strategy: round-robin # atau consistent-hashing
  proxies: # ini bisa mengarah ke proxy group lain atau langsung di akun yang ada di config
  - trojan
  - vmess
  - vless
  - shadowsocks
  use: # ini di peruntukkan untuk jalur proxy provider
  - wan
  - wanb
  url: http://www.gstatic.com/generate_204
  interval: 99
```

{% include links.html %}