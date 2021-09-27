<p align="right">En | <a href="../README.md">En</a>
<div align="center">
<h1>nmgp</h1>
轻松地通过nmgp在macOS上使用http全局代理，并且使用mitmproxy来监听这些请求。
[![GitHub release](https://img.shields.io/github/v/release/newtorn/nmgp)](https://github.com/newtorn/nmgp/releases)
[![Github repository](https://img.shields.io/appveyor/build/newtorn/https://github.com/newtorn/nmgp.git)](https://github.com/newtorn/nmgp.git)
[![Github license](https://img.shields.io/github/license/newtorn/nmgp.git)](LICENSE)
</div>
</p>


## About

[nmgp](https://github.com/newtorn/nmgp.git)是一个macOS全局代理设置工具，https代理证书使用mitmproxy证书。设置mitmproxy http代理时，流量会经过mtimproxy，通常用来监听http请求或者抓包。由于需要使用mitmproxy监听请求，所以首先安装mitmproxy，默认采用brew方式安装，HTTPS依赖CA证书，否则mitmproxy无法监听HTTPS请求。


## Installation

很容易通过下面的方式安装它。

#### MacOS
使用Homebrew安装它。
```
brew tap newtorn/tap && brew install nmgp
```

#### Linux
使用脚本源代码安装它。
```
curl https://raw.githubusercontent.com/newtorn/nmgp/master/src/nmgp >> /bin/nmgp && chmod +x /bin/nmgp
```


## Usage

```
# 设置mitmproxy代理的host和port
nmgp set 127.0.0.1 8080

# 开启全局代理
nmgp on

# 关闭全局代理
nmgp off

# curl测试代理
curl http://www.xxx.com

# 浏览器测试代理
# app测试代理

# 获取帮助
nmgp help
```

## Contributing

我很热爱你为newgo贡献，请阅读我的[贡献指南](../CONTRIBUTING.md)


## License

代码使用 [MIT](../LICENSE) 声明
