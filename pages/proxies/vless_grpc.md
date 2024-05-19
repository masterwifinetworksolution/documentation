---
title: Vless GRPC
tags: [proxies]
keywords: account, proxies, clash
summary: "Akun clash vless grpc."
sidebar: clash
permalink: vless_grpc.html
folder: proxies
comments: false
toc: false
---

```yaml
- name: Vless gRPC (SNI)
  server: SERVER.COM
  port: 443
  type: vless
  uuid: UUID
  cipher: auto
  tls: true
  skip-cert-verify: true
  servername: BUGSNI.COM
  network: grpc
  grpc-opts:
  grpc-mode: gun
  grpc-service-name: NAMAGRPC
  udp: true
```

{% include links.html %}