pyweaknet
========

A limited network transport implementation in PYTHON.

# Install

## pip

``` sh
pip install weaknet
```

## direct file

``` sh
cd <you execute path>
curl -O https://raw.githubusercontent.com/vietor/pyweaknet/master/bin/weaknet.py
```

# Usage

Just *onefile* for provider all service.

Require:
> python >= 2.6, compatible 3.x

Recommend:
> openssl for most crypto.  
> sodium for chacha20 & salsa20

More discritption:
```sh
weaknet.py --help
```

## Role: remote

A modifyed socket proxy server, compatible *shadowsocks* protocol.
> default bind port: 58080

## Role: local

A wrappered proxy server, multiple protocal support.
> default bind port 51080  
> --shadowsocks for direct usage *shadowsocks* server.  
> --rulelist compatible gfwlist format

### SOCKS4
Direct usage.

### SOCKS4A
Direct usage.

### SOCKS5
Direct usage. Unsupoort authentication.

### HTTP PROXY
Direct usage. Unsupoort authentication.

### AUTO PROXY
Usage like "http://127.0.0.1:51080/proxy.pac". Unsupoort authentication.


