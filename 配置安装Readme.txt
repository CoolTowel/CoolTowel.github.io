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
