---
title: Trojan Websocket
tags: [proxies]
keywords: account, proxies, clash
summary: "Akun clash trojan ws."
sidebar: clash
permalink: trojan_ws.html
folder: proxies
comments: false
toc: false
---

## SNI

```yaml
proxies:
- name: Trojan WS (SNI)
  server: SERVER.COM
  port: 443
  type: trojan
  password: PASSWORD
  skip-cert-verify: true
  sni: BUGSNI.COM
  network: ws
  ws-opts:
    path: /PATH
    headers:
      Host: BUGSNI.COM
  udp: true
```

## CDN

```yaml
proxies:
- name: Trojan GO/WS (CDN)
  server: IPCDN/BUGCDN.COM
  port: 443
  type: trojan
  password: PASSWORD
  network: ws
  sni: SERVER.COM
  skip-cert-verify: true
  udp: true
  ws-opts:
    path: /PATH
    headers:
        Host: SERVER.COM
```

{% include links.html %}