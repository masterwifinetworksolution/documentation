---
title: Vmess GRPC
tags: [proxies]
keywords: account, proxies, clash
summary: "Akun clash vmess grpc."
sidebar: clash
permalink: vmess_grpc.html
folder: proxies
comments: false
toc: false
---

```yaml
- name: Vmess gRPC (SNI)
  server: SERVER.COM
  port: 443
  type: vmess
  uuid: UUID
  alterId: 0
  cipher: auto
  network: grpc
  tls: true
  servername: BUGSNI.COM
  skip-cert-verify: true
  grpc-opts:
    grpc-service-name: NAMAGRPC
```

{% include links.html %}