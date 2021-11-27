
除node外均同步至 source branch，无需备份。
需要插件：
    hexo-deployer-git
        安装：npm install hexo-deployer-git --save
        随后还需在_config中修改参数，详见hexo文档
    hexo-optimize
    
此外还对Next主题css文档做了一些更改，例如site-title的字号大小。

    在 themes/next/source/css/_schemes/Pisces/_header.styl 文件中的 .site-meta 中添加 .site-title{} 设定值：
    .site-meta {
    padding: 20px 0;
    .site-title {
        font-size: 250%;
    }
    }

HEXO 及 NEXT 主题版本：（2021-11-27）

hexo --version
INFO  Validating config
INFO  ==================================
  ███╗   ██╗███████╗██╗  ██╗████████╗
  ████╗  ██║██╔════╝╚██╗██╔╝╚══██╔══╝
  ██╔██╗ ██║█████╗   ╚███╔╝    ██║
  ██║╚██╗██║██╔══╝   ██╔██╗    ██║
  ██║ ╚████║███████╗██╔╝ ██╗   ██║
  ╚═╝  ╚═══╝╚══════╝╚═╝  ╚═╝   ╚═╝
========================================
NexT version 8.8.0
Documentation: https://theme-next.js.org
========================================
hexo: 5.4.0
hexo-cli: 4.3.0
os: darwin 21.1.0 12.0.1

node: 16.13.0
v8: 9.4.146.19-node.13
uv: 1.42.0
zlib: 1.2.11
brotli: 1.0.9
ares: 1.18.0
modules: 93
nghttp2: 1.46.0
napi: 8
llhttp: 6.0.4
openssl: 1.1.1l
cldr: 39.0
icu: 69.1
tz: 2021a
unicode: 13.0