---
title: Select
tags: [proxy_groups]
keywords: proxy groups, select, clash
summary: "Proxy groups select clash."
sidebar: clash
permalink: proxy_groups_select.html
folder: proxy groups
comments: false
toc: false
---

```yaml
proxy-groups:
- name: Select
  type: select
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