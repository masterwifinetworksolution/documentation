---
title: Failover
tags: [proxy_groups]
keywords: proxy groups, fallback, clash
summary: "Proxy groups fallback clash."
sidebar: clash
permalink: proxy_groups_fallback.html
folder: proxy groups
comments: false
toc: false
---

```yaml
proxy-groups:
- name: FAILOVER
  type: fallback
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