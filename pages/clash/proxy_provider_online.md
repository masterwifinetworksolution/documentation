---
title: Proxy Provider Online
tags: [clash]
keywords: proxy provider, online, clash
summary: "Proxy provider online clash."
sidebar: clash
permalink: proxy_provider_online.html
folder: clash
comments: false
toc: false
---

```yaml
proxy-providers:
  Provider-Online:
    type: http
    url: https://alamat-akun-online.yaml
    path: ./proxy_provider/akun-online.yaml
    interval: 3600
    health-check:
      enable: true
      url: http://www.gstatic.com/generate_204
      interval: 99
```

{% include links.html %}