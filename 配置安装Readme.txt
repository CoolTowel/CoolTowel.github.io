
需要插件：

    hexo-deployer-git
        安装：npm install hexo-deployer-git --save
        随后还需在_config中修改参数，详见hexo文档
    
    hexo-optimize

    npm install hexo-lazyload-image --save
    
此外还对Next主题做了一些更改，例如site-title的字号大小。

    在 ./source/_data中添加styles.styl文件，并在 ./_config.next.yml 中 custom_file_path 项中添加该文件以生效。（styles.styl中的配置会覆盖.theme/next/source/css/文件夹中的配置)

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