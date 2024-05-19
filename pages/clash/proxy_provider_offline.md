---
title: Proxy Provider Offline
tags: [clash]
keywords: proxy provider, offline, clash
summary: "Proxy provider offline clash."
sidebar: clash
permalink: proxy_provider_offline.html
folder: clash
comments: false
toc: false
---

```yaml
proxy-providers:
  Provider-Offline:
    type: file
    path: ./proxy_provider/akun.yaml
    health-check:
      enable: true
      url: http://www.gstatic.com/generate_204
      interval: 99
```

{% include links.html %}