---
layout: page
title: Vless GRPC
permalink: "/vless-grpc/"
image: assets/images/file.jpg
---

```
proxies:
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