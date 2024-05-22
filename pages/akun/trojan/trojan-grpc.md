---
layout: page
title: Trojan GRPC
permalink: "/trojan-grpc/"
image: assets/images/file.jpg
---

```
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