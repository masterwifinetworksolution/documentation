---
title:  "Membuat akun clash"
categories: Account
permalink: membuat-akun-clash.html
tags: [clash]
summary: Cara membuat dan menambahkan akun di dalam clash
toc: true
---

**Cara agar koneksi anda bisa berjalan dengan normal, maka diperlukan sebuah akun untuk memproses semua kinerja pada proxy provider hingga ke ruleset Antara Proxy Group dan Rule atau Script.**

Dan berikut ini akan kami rangkumkan semua akun agar bisa anda gunakan dalam sehari-hari.

## Trojan GFW SNI

```yaml
proxies:
- name: Trojan GFW (SNI)
  type: trojan
  server: SERVER.COM
  port: 443
  password: PASSWORD
  udp: true
  sni: BUGSNI.COM
  skip-cert-verify: true
```

### Trojan WS SNI

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

### Trojan Go CDN

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

### Trojan XTLS

```yaml
- name: Trojan XTLS SNI
  server: SERVER.COM
  port: 443
  type: trojan
  password: PASSWORD
  flow: xtls-rprx-direct
  skip-cert-verify: true
  sni: BUGSNI.COM
  udp: true
```

### Trojan GRPC SNI

```yaml
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

### Vmess WS SNI

```yaml
- name: Vmess WS (SNI)
  type: vmess
  server: SERVER.COM
  port: 443
  uuid: UUID
  alterId: 0
  cipher: auto
  udp: true
  tls: true
  skip-cert-verify: true
  servername: BUGSNI.COM
  network: ws
  ws-opts:
    path: /PATH
    headers:
      Host: BUGSNI.COM
```

### Vmess WS CDN

```yaml
- name: Vmess WS (CDN)
  type: vmess
  server: IPCDN/BUGCDN.COM
  port: 443
  uuid: UUID
  alterId: 0
  cipher: auto
  udp: true
  tls: true
  skip-cert-verify: true
  servername: SERVER.COM
  network: ws
  ws-opts:
    path: /PATH
    headers:
      Host: SERVER.COM
```

### Vmess WS CDN Tanpa TLS

```yaml
- name: Vmess WS (CDN) Non TLS
  type: vmess
  server: IPCDN/BUGCDN.COM
  port: 80
  uuid: UUID
  alterId: 0
  cipher: auto
  udp: true
  tls: false
  skip-cert-verify: false
  servername: SERVER.COM
  network: ws
  ws-opts:
    path: /PATH
    headers:
      Host: SERVER.COM
```

### Vmess GRPC SNI

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

### Vless WS SNI

```yaml
- name: Vless WS (SNI)
  server: SERVER.COM
  port: 443
  type: vless
  uuid: UUID
  cipher: auto
  tls: true
  skip-cert-verify: true
  servername: BUGSNI.COM
  network: ws
  ws-opts:
    path: /PATH
    headers:
      Host: BUGSNI.COM
```

### Vless WS CDN

```yaml
- name: Vless WS (CDN)
  server: IPCDN/BUGCDN.COM
  port: 443
  type: vless
  uuid: UUID
  cipher: auto
  tls: true
  skip-cert-verify: true
  servername: SERVER.COM
  network: ws
  ws-opts:
    path: /PATH
    headers:
      Host: SERVER.COM
```

### Vless WS CDN Tanpa TLS

```yaml
- name: Vless WS (CDN) Non TLS
  server: IPCDN/BUGCDN.COM
  port: 80
  type: vless
  uuid: 81f1f510-3ca7-4734-8956-0f4fce670af5
  cipher: auto
  tls: false
  skip-cert-verify: false
  servername: SERVER.COM
  network: ws
  ws-opts:
    path: /PATH
    headers:
      Host: SERVER.COM
  udp: true
```

### Vless XTLS SNI

```yaml
- name: Vless XTLS (SNI)
  server: SERVER.COM
  port: 443
  type: vless
  uuid: UUID
  cipher: auto
  tls: true
  flow: xtls-rprx-direct
  skip-cert-verify: true
  servername: BUGSNI.COM
```

### Vless GRPC SNI

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

### Socks5 SNI

```yaml
- name: Socks5 (SNI)
  type: socks5
  server: SERVER.COM
  port: 443
  username: USERNAME
  password: PASSWORD
  tls: true
  skip-cert-verify: true
  udp: true
  sni: BUGSNI.COM
```

### Shadowsocks Tanpa Plugin

```yaml
- name: Shadowsocks Tanpa Plugin
  type: ss
  server: SERVER.COM
  port: 34963
  cipher: chacha20-ietf-poly1305
  password: PASSWORD
  udp: true
```

### Shadowsocks Plugin OBFS

```yaml
- name: Shadowsocks Plugin Obfs
  type: ss
  server: SERVER.COM
  port: 32033
  cipher: chacha20-ietf-poly1305
  password: PASSWORD
  plugin: obfs
  plugin-opts:
    mode: tls
    host: BUGSNI.COM
```

### ShadowsocksR SNI

```yaml
- name: ShadowsocksR (SNI)
  server: SERVER.COM
  port: 1235
  type: ssr
  cipher: AES-256-CTR
  password: PASSWORD
  protocol: origin
  obfs: tls1.2_ticket_auth
  protocol-param: "#"
  obfs-param: BUGSNI.COM
  udp: true
```

### Snell Support UDP

```yaml
- name: Snell V3
  type: snell
  server: SERVER.COM
  port: 33223
  psk: PASSWORD
  version: 3
  udp: true
  obfs-opts:
    mode: tls
    host: BUGSNI.COM
```

Semua akun ini bisa diterapkan pada:

- [Openclash](openclash)
- [Clash For Android](/android)
- [Clash For Magisk](/magisk)
- [Box For Magisk](/bfm)
- [Clash For Linux](/linux)
- [Clash For Windows](/windows)

Dan masih banyak yang lain nya untuk type Clash.

{% include links.html %}