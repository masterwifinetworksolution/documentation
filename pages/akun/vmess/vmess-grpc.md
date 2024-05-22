---
layout: page
title: Vmess GRPC
permalink: "/vmess-grpc/"
image: assets/images/file.jpg
---

```
proxies:
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