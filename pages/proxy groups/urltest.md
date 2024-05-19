---
title: Best Ping
tags: [proxy_groups]
keywords: proxy groups, url test, clash
summary: "Proxy groups url test clash."
sidebar: clash
permalink: proxy_groups_urltest.html
folder: proxy groups
comments: false
toc: false
---

```yaml
proxy-groups:
- name: Best Ping
  type: url-test
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