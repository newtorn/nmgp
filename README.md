<p align="right">En | <a href="./doc/README-zh_cn.md">中文</a></p>
<div align="center">

### nmgp

Easily use mitmproxy global http proxy on your macOS with nmgp

[![GitHub release](https://img.shields.io/github/v/release/newtorn/nmgp)](https://github.com/newtorn/nmgp/releases)
[![Github repository](https://img.shields.io/appveyor/build/newtorn/https://github.com/newtorn/nmgp.git)](https://github.com/newtorn/nmgp.git)
[![Github license](https://img.shields.io/github/license/newtorn/nmgp.git)](LICENSE)

</div>

## About

[nmgp](https://github.com/newtorn/nmgp.git) is a macOS mitmproxy global http proxy tool.Set global http proxy, the network data will fallthough mitmproxy, it is used to monitor or capture data packet.Proxy service listener with mitmproxy, so first step is that install mitmproxy, default to brew install it, protocol HTTPS in mitmproxy dependences mitm CA certification, set the proxy with ca cert.


## Installation

It's easy to be installed.

#### MacOS
You can use homebrew to install it.
```
brew tap newtorn/tap && brew install nmgp
```

#### Linux
You should download or copy [nmgp](https://github.com/newtorn/nmgp.git) shell script.
```
curl https://raw.githubusercontent.com/newtorn/nmgp/master/src/nmgp >> /bin/nmgp && chmod +x /bin/nmgp
```

## Usage

```
# first set proxy host port
nmgp set 127.0.0.1 8080

# set proxy on
nmgp on

# set proxy off

# test proxy by curl
curl http://www.xxx.com

# test proxy by browser
# test app network packet

# Get help
nmgp help
```

## Contributing

I'd love you to contribute to nmgp, please read my [Contribution Guide](CONTRIBUTING.md)


## License

Code license with [MIT](LICENSE)
