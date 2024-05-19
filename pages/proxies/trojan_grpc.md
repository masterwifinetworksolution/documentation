---
title: Trojan GRPC
tags: [proxies]
keywords: account, proxies, clash
summary: "Akun clash trojan grpc."
sidebar: clash
permalink: trojan_grpc.html
folder: proxies
comments: false
toc: false
---

```yaml
proxies:
- name: Trojan gRPC (SNI)
  type: trojan
  server: SERVER.COM
  port: 443
  password: PASSWORD
  udp: true
  sni: BUGSNI.COM
  skip-cert-verify: true
  network: grpc
  grpc-opts:
    grpc-service-name: NAMAGRPC
```

{% include links.html %}