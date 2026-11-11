# WireGuard 配置
proxies:
  - name: "🔐 WG内网"
    type: wireguard
    server:  # WG服务器IP或域名
    port: 51820
    ip: 10.0.0.2/24
    private-key: ""       # 客户端私钥
    public-key: ""        # 服务器公钥
    pre-shared-key: ""    # 预共享密钥
    allowed-ips:
      - 0.0.0.0/0
      - ::/0
    persistent-keepalive: 25
    mtu: 1420
    udp: true
